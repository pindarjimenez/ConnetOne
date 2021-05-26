<template>
    <b-card no-body class="announcements">
        <b-card-body class="px-2">
            <div class="px-4">
                <b-card-img src="https://placekitten.com/200/200" alt="Image" class="rounded-circle"></b-card-img>
            </div>
            <b-card-title class="text-center mt-4 mb-0">Sparkle d'Cat</b-card-title>
            <b-card-text class="motto">
               Proin ut augue at dui cursus sit amet vitae.
            </b-card-text>
            <b-row class="mx-1 mt-4 activity">
                <b-col class="px-1">
                    <b-card no-body bg-variant="light" class="text-center item">
                        <div class="total">12</div>
                        <div class="title">Posts</div>
                    </b-card>
                </b-col>
                <b-col class="px-1">
                    <b-card no-body bg-variant="light" class="text-center item">
                        <div class="total">5</div>
                        <div class="title">Mentions</div>
                    </b-card>
                </b-col>
                <b-col class="px-1">
                    <b-card no-body bg-variant="light" class="text-center item">
                        <div class="total">8</div>
                        <div class="title">Shared</div>
                    </b-card>
                </b-col>
            </b-row>
        </b-card-body>
    </b-card>  
</template>

<style lang="scss" scoped>
    .motto {
        position: relative;
        margin-top: 10px;
        margin-left: 20px;
        font-style: italic;

        &::before {
            font-family: "Times New Roman", Times, serif;
            position: absolute;
            left: -18px;
            top: -5px;
            font-weight: 800;
            font-size: 30px;
            content: '\201C';
        }
    }

    .activity {
        .item {
            padding-top: 5px;
            padding-bottom: 5px;

            .total {
                font-weight: 800;
            }

            .title {
                font-size: 12px;
            }
        }
    }
</style>