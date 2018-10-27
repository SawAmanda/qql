<!-- 首页 合作媒体 组件 -->
<template>
    <section class="media">
        <div class="media_outside">
            <div class="media_bg">
                <img src="../../../static/images/home/media_background.png" alt="">
            </div>
            <div class="media_inside_box">
                <div class="media_inside">
                    <div class="media_title">
                        <p>合作媒体</p>
                    </div>
                    <div class="media_logo">
                        <ul>
                            <li v-for="media in logoList">
                                <img :src="media.logourl" alt="">
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            logoList: [
                {
                    mediaID : 1,
                    name: "腾讯",
                    logourl: './static/images/home/media_01.png'
                },
                {
                    mediaID : 2,
                    name: "腾讯",
                    logourl: './static/images/home/media_02.png'
                },
                {
                    mediaID : 3,
                    name: "腾讯",
                    logourl: './static/images/home/media_01.png'
                },
                {
                    mediaID : 4,
                    name: "腾讯",
                    logourl: './static/images/home/media_02.png'
                },
                {
                    mediaID : 5,
                    name: "腾讯",
                    logourl: './static/images/home/media_01.png'
                },
                {
                    mediaID : 6,
                    name: "腾讯",
                    logourl: './static/images/home/media_02.png'
                },
                {
                    mediaID : 7,
                    name: "腾讯",
                    logourl: './static/images/home/media_01.png'
                },
                {
                    mediaID : 8,
                    name: "腾讯",
                    logourl: './static/images/home/media_02.png'
                },
                {
                    mediaID : 9,
                    name: "腾讯",
                    logourl: './static/images/home/media_01.png'
                },
                {
                    mediaID : 10,
                    name: "腾讯",
                    logourl: './static/images/home/media_02.png'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../../dependencies/sass/style.scss';

.media {
    width: 100%;
    overflow: hidden;
    .media_outside {
        height: vm(476);
        position: relative;
        .media_bg {
            width: 100%;
            height: 100%;
            position: absolute;
            top: 0;
            left: 0;
            z-index: 1;
        }
        .media_inside_box {
            width: 100%;
            height: 100%;
            z-index: 2;
            position: absolute;
            top: 0;
            left: 0;
            .media_inside {
                width: vm(1200);
                margin: 0 auto;
                .media_title {
                    margin-top: vm(105);
                    p {
                        color: #000;
                        font-size: vm(26);
                        text-align: center;
                        letter-spacing: vm(1);
                    }
                }
                .media_logo {
                    margin-top: vm(43);
                    ul {
                        display: flex;
                        flex-wrap: wrap;
                        justify-content: space-between;
                        align-content: center;
                        li {
                            width: vm(220);
                            height: vm(82);
                            margin-right: vm(16);
                            margin-top: vm(17);
                            &:nth-child(5),&:last-child {
                                margin-right: 0;
                            }
                        }
                    }
                }
            }
        }
    }
}

</style>

