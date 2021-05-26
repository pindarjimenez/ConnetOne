<template>
    <b-card class="post">
        <b-card-text class="title">Start a Post</b-card-text>
        <b-form-input placeholder="Write something..."></b-form-input>
        <div class="actions">
            <div class="item"><b-icon icon="images" class="mr-2"></b-icon>Photo/Video</div>
            <div class="item"><b-icon icon="share-fill" class="mr-2"></b-icon>Share</div>
            <div class="item"><b-icon icon="calendar3" class="mr-2"></b-icon>Event</div>
        </div>
    </b-card>  
</template>

<style lang="scss" scoped>
    .post {
        .title {
            font-weight: 600;
            margin-bottom: 5px;
        }

        .actions {
            color: #707070;
            display: flex;
            margin-top: 10px;

            .item {
                font-weight: 600;
                font-size: 14px;
                margin-right: 15px;
                cursor: pointer;

                &:hover {
                    color: #7cabd1;
                }
            }
        }
    }
</style>