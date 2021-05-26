<template>
    <b-card no-body class="story">
        <b-row class="px-2">
            <b-col class="px-1">
                <div class="create-story">
                    <b-icon variant="secondary" icon="images" font-scale="3"></b-icon>
                    <div class="title">Create Story</div>
                    <div class="description">Events, activities, news, birthdays, etc.</div>
                </div>
            </b-col>
            <b-col class="px-1">
                <div class="create-story">
                    <b-icon variant="secondary" icon="image-alt" font-scale="5" class="mt-5"></b-icon>
                </div>
            </b-col>
            <b-col class="px-1">
                <div class="create-story">
                    <b-icon variant="secondary" icon="image-alt" font-scale="5" class="mt-5"></b-icon>
                </div>
            </b-col>
        </b-row>
        <b-avatar 
            variant="dark" 
            size="2.1rem" 
            icon="arrow-right" 
            v-b-tooltip.hover.top 
            title="View More Stories"
            class="more-stories"
        ></b-avatar>
    </b-card>  
</template>

<style lang="scss" scoped>
    .story {
        position: relative;
        padding: 15px;

        .create-story {
            padding: 25px 5px;
            text-align: center;
            background-color: #F1F1F1;
            color: #707070;
            height: 100%;
            vertical-align: middle;

            .title {
                margin-top: 15px;
                font-size: 15px;
                font-weight: 600;
            }

            .description {
                margin-top: 5px;
                font-size: 12px;
                font-style: italic;
            }
        }

        .more-stories {
            position: absolute;
            margin-top: auto;
            margin-bottom: auto;
            top: 0;
            bottom: 0; 
            right: -10px;
            cursor: pointer;

            &:hover {
                color: #7cabd1;
            }
        }
    }
</style>