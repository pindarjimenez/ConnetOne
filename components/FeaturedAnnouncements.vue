<template>
    <b-card no-body>
        <template v-for="(announcement, index) in announcements">
            <b-row no-gutters :key="index" v-show="activeFeatured == index">
                <b-col md="5">
                    <b-card-img :src="announcement.img" alt="Image" class="rounded-0"></b-card-img>
                </b-col>
                <b-col md="7">
                    <b-card-body class="p-3 d-flex flex-column h-100">
                        <b-card-text class="text-right small text-muted">{{ index + 1 }} of 3</b-card-text>
                        <b-card-text class="small text-muted mb-0">2021.05.21</b-card-text>
                        <b-card-title class="mb-1">{{ announcement.title }}</b-card-title>
                        <announcement-icons></announcement-icons>
                        <b-card-text>{{ announcement.desc }}</b-card-text>
                        <div class="mt-auto text-right">
                            <b-avatar button variant="dark" size="1.3rem" icon="chevron-left" @click="activeFeatured = (index != 0 ? index - 1 : index)"></b-avatar>
                            <b-avatar button variant="dark" size="1.3rem" icon="chevron-right" @click="activeFeatured = (index != 2 ? index + 1 : index)"></b-avatar>
                        </div>
                    </b-card-body>
                </b-col>
            </b-row>
        </template>
    </b-card>    
</template>

<script>
export default {
    data() {
        return {
            announcements: [
                {
                    'img': 'https://picsum.photos/300/600/?image=22',
                    'title': 'Lorem ipsum dolor',
                    'desc': 'Cras egestas maximus velit, sit amet ultricies metus lobortis luctus. Nullam gravida velit porta, semper nunc ac, condimentum arcu. Integer dapibus ex sit amet odio...'
                },
                {
                    'img': 'https://picsum.photos/300/600/?image=23',
                    'title': 'Nulla quis lorem',
                    'desc': 'Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula...'
                },
                {
                    'img': 'https://picsum.photos/300/600/?image=24',
                    'title': ' Curabitur arcu',
                    'desc': 'Quisque velit nisi, pretium ut lacinia in, elementum id enim. Nulla porttitor accumsan tincidunt...'
                },

            ],
            activeFeatured: 0
        }
    },
}
</script>

<style lang="scss">
    .b-avatar-img {
        padding: 2px; 

        img {
            object-fit: inherit !important;
        }
    }

    .card-title {
        font-size: 20px;
    }
</style>