<template>
    <b-card no-body class="announcements">
        <b-card-header class="d-flex justify-content-between align-items-center">
            <h4>Announcements</h4>
            <b-link href="#" class="card-link">View All</b-link>
        </b-card-header>

        <b-card-body>
            <div class="items" v-for="(announcement, index) in announcements" :key="index">
                <b-card-text class="small text-muted mb-0">{{ announcement.date }}</b-card-text>
                <b-card-title class="mb-1">{{ announcement.title }}</b-card-title>
                <announcement-icons></announcement-icons>
                <b-card-text>{{ announcement.desc }}</b-card-text>
            </div>
        </b-card-body>
    </b-card>  
</template>

<script>
export default {
    data() {
        return {
            announcements: [
                {
                    'title': 'Lorem ipsum dolor',
                    'date': '2021.05.15',
                    'desc': 'Cras egestas maximus velit, sit amet ultricies metus lobortis luctus. Nullam gravida velit porta, semper nunc ac, condimentum arcu. Integer dapibus ex sit amet odio...'
                },
                {
                    'title': 'Nulla quis lorem',
                    'date': '2021.05.16',
                    'desc': 'Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula...'
                },
                {
                    'title': 'Curabitur arcu',
                    'date': '2021.05.17',
                    'desc': 'Quisque velit nisi, pretium ut lacinia in, elementum id enim. Nulla porttitor accumsan tincidunt...'
                },
                {
                    'title': 'Vivamus magna',
                    'date': '2021.05.17',
                    'desc': 'Vivamus suscipit tortor eget felis porttitor volutpat. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus....'
                },
                {
                    'title': 'Donec sollicitudin',
                    'date': '2021.05.18',
                    'desc': 'Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. ....'
                },
                {
                    'title': 'Molestie malesuada.',
                    'date': '2021.05.20',
                    'desc': 'Eget tincidunt nibh pulvinar. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus...'
                },
                {
                    'title': 'Quisque velit',
                    'date': '2021.05.23',
                    'desc': 'Cras egestas maximus velit, sit amet ultricies metus lobortis luctus. Nullam gravida velit porta, semper nunc ac, condimentum arcu. Integer dapibus ex sit amet odio...'
                },
                {
                    'title': 'Nulla quis lorem',
                    'date': '2021.05.24',
                    'desc': 'Quisque velit nisi, pretium ut lacinia in, elementum id enim. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a...'
                },
                {
                    'title': 'Proin ege',
                    'date': '2021.05.25',
                    'desc': 'Proin eget tortor risus. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Sed porttitor lectus nibh...'
                },
            ],
            activeFeatured: 0
        }
    },
}
</script>

<style lang="scss">
    .announcements {
        .b-avatar-img {
            padding: 2px; 

            img {
                object-fit: inherit !important;
            }
        }

        .card-title {
            font-size: 20px;
        }

        .card-body {
            max-height: 600px;
            overflow-y: auto;

            .items {
                padding: 15px 0;

                &:first-child {
                    padding-top: 0;
                }

                &:not(:last-child) {
                    border-bottom: 1px solid #000;
                }
            }
        }
    }
</style>