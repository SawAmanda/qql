<!-- 首页 主营业务 组件 尚未开发完成 -->
<template>
    <section class="mainness">
        <div class="mness_outside">
            <div class="mness_inside">
                <ul class="mness_">
                    <li v-for="mness in mnesslist">
                        <div class="mness_imgText">
                            <img src="../../../static/images/home/yewu/yewu_01.png" alt="">
                            <p> {{mness.title}} </p>
                        </div>
                        <p class="mness_content">{{mness.content}}</p>
                        <div class="mness_hover">
                            <div class="hover_box">
                                <div class="hover_keywords">
                                    <div class="keywords_bg">
                                        <img src="../../../static/images/home/yewu/yewu_bg2.png" alt="">
                                        <p>关键词</p>
                                    </div>
                                    
                                </div>
                                <ul>
                                    <li>
                                        <div class="hover_text_box">
                                            <p>区块链+</p>
                                        </div>
                                        <div class="hover_text_box">
                                            <p>区块链+</p>
                                        </div>
                                        <div class="hover_text_box">
                                            <p>区块链+</p>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            mnesslist: [
                {
                    img: './static/images/home/yewu/yewu_01.png',
                    title: '技术开发',
                    content: '专业开发团队，在区块链+领域拥有丰富经验，根据企业需求定制开发官网、APP、小程序、微商城等平台，同时提供用户自传播的营销工具。'
                },
                {
                    img: './static/images/home/yewu/yewu_02.png',
                    title: '项目运维',
                    content: '团队具有广泛的行业经验以及广阔的产业、渠道资源。运维实操过程结合各行业发展趋势和业务特点，进行精准化市场营销、运营，实现项目成功增值。'
                },
                {
                    img: './static/images/home/yewu/yewu_03.png',
                    title: '创业投资',
                    content: '轻起来集团拥有雄厚的资金实力与管理经验。依据敏锐的商业眼光，发掘有潜力的合作项目并乐于对其进行资金、管理等方面的扶持，达成合作共赢。'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../../dependencies/sass/style.scss';

.mainness {
    width: 100%;
    position: absolute;
    top: vm(517);
    z-index: 2;
    .mness_outside {
        .mness_inside {
            width: vm(1200);
            margin: 0 auto;
            background: #fff;
            ul {
                display: flex;
                justify-content: space-between;
                li {
                    width: vm(380);
                    padding: 0 vm(30) 0 vm(35);
                    position: relative;
                    &:hover .mness_hover {
                        display: block;
                    }
                    .mness_imgText {
                        margin: vm(53) auto vm(24) auto;
                        img {
                            width: vm(67);
                            margin: 0 auto;
                        }
                        p {
                            font-size: vm(24);
                            color: #3eaad7;
                            text-align: center;
                        }
                    }
                    .mness_content {
                        font-size: vm(16);
                        padding-bottom: vm(75);
                    }
                    .mness_hover {
                        width: 100%;
                        height: 100%;
                        position: absolute;
                        top: 0;
                        left: 0;
                        background: url("../../../static/images/home/yewu/yewu_bg.png");
                        display: none;
                        .hover_box {
                            width: vm(200);
                            height: 100%;
                            margin: 0 auto;
                            overflow: hidden;
                            .hover_keywords {
                                width: 100%;
                                position: relative;
                                .keywords_bg {
                                    width: 100%;
                                    padding-top: vm(73);
                                }
                                p {
                                    color: #fff;
                                    font-size: vm(22);
                                    position: absolute;
                                    top: vm(60);
                                    width: 100%;
                                    text-align: center;
                                }
                            }
                            ul {
                                flex-direction: column;
                                flex-wrap: wrap;
                                margin-top: vm(35);
                                li {
                                    float: none;
                                    width: vm(200);
                                    padding: 0;
                                    .hover_text_box {
                                        width: 100%;
                                        height: vm(36);
                                        background: url("../../../static/images/home/yewu/yewu_k.png");
                                        background-size: 100% 100%;
                                        background-repeat: no-repeat;
                                        margin-bottom: vm(35);
                                        p {
                                            text-align: center;
                                            color: #fff;
                                            line-height: vm(36);
                                        }
                                    }
                                    
                                }
                            }
                        }
                    }
                }
            }
        }
    }
}
</style>

