<template>
    <b-card no-body class="news-feed">
        <b-card-title class="text-primary">News Feed</b-card-title>
        <b-card-body>
            <div class="item" v-for="(feed, index) in newsfeed" :key="index">
                <div class="header">
                    <b-avatar href="#" :src="feed.img"></b-avatar>
                    <div class="details">
                        <div class="name">{{ feed.name }}</div>
                        <div class="date">{{ feed.date }}</div>
                    </div>
                </div>
                <div class="content">
                    {{ feed.content }}
                </div>
                <div class="footer">
                    <div class="item"><b-icon icon="hand-thumbs-up" class="mr-2"></b-icon>Like</div>
                    <div class="item"><b-icon icon="chat-left" class="mr-2"></b-icon>Comment</div>
                    <div class="item"><b-icon icon="share-fill" class="mr-2"></b-icon>Share</div>
                </div>
            </div>
        </b-card-body>
    </b-card>  
</template>

<script>
export default {
    data() {
        return {
            newsfeed: [
                {
                    'img': 'https://picsum.photos/300/300/?image=1',
                    'name': 'John Doe',
                    'date': '2021.05.15',
                    'content': 'Cras egestas maximus velit, sit amet ultricies metus lobortis luctus. Nullam gravida velit porta, semper nunc ac, condimentum arcu. Integer dapibus ex sit amet odio...'
                },
                {
                    'img': 'https://picsum.photos/300/300/?image=12',
                    'name': 'Nulla quis lorem',
                    'date': '2021.05.16',
                    'content': 'Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula...'
                },
                {
                    'img': 'https://picsum.photos/300/300/?image=3',
                    'name': 'Curabitur arcu',
                    'date': '2021.05.17',
                    'content': 'Quisque velit nisi, pretium ut lacinia in, elementum id enim. Nulla porttitor accumsan tincidunt...'
                },
                {
                    'img': 'https://picsum.photos/300/300/?image=4',
                    'name': 'Vivamus magna',
                    'date': '2021.05.17',
                    'content': 'Vivamus suscipit tortor eget felis porttitor volutpat. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus....'
                },
                {
                    'img': 'https://picsum.photos/300/300/?image=25',
                    'name': 'Donec sollicitudin',
                    'date': '2021.05.18',
                    'content': 'Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. ....'
                },
                {
                    'img': 'https://picsum.photos/300/300/?image=36',
                    'name': 'Molestie malesuada.',
                    'date': '2021.05.20',
                    'content': 'Eget tincidunt nibh pulvinar. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus...'
                },
                {
                    'img': 'https://picsum.photos/300/300/?image=47',
                    'name': 'Quisque velit',
                    'date': '2021.05.23',
                    'content': 'Cras egestas maximus velit, sit amet ultricies metus lobortis luctus. Nullam gravida velit porta, semper nunc ac, condimentum arcu. Integer dapibus ex sit amet odio...'
                },
                {
                    'img': 'https://picsum.photos/300/300/?image=8',
                    'name': 'Nulla quis lorem',
                    'date': '2021.05.24',
                    'content': 'Quisque velit nisi, pretium ut lacinia in, elementum id enim. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a...'
                },
                {
                    'img': 'https://picsum.photos/300/300/?image=9',
                    'name': 'Proin ege',
                    'date': '2021.05.25',
                    'content': 'Proin eget tortor risus. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Sed porttitor lectus nibh...'
                },
            ],
            activeFeatured: 0
        }
    },
}
</script>

<style lang="scss" scoped>
    .news-feed {
        padding: 15px;
        
        .card-body {
            max-height: 810px;
            overflow-y: auto;

            > .item {
                border: 1px solid #707070;
                padding: 15px;
                border-radius: 5px;
                background-color: #eee;
                margin-bottom: 15px;

                .header {
                    display: flex;
                    margin-bottom: 15px;

                    .details {
                        margin-left: 10px;
                        .name {
                            font-weight: 600;
                        }

                        .date {
                            font-size: 10px;
                        }
                    }
                }

                .content {
                    margin-bottom: 15px;
                }

                .footer {
                    display: flex;
                    justify-content: space-around;
                    border-top: 1px solid #707070;
                    padding-top: 15px;

                    .item:hover {
                        color: #7cabd1;
                    }
                }
            }
        }
    }
</style>