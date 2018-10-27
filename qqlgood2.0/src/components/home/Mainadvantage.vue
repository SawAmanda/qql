<!-- 首页 轻起来业务优势 组件-->
<template>
    <section class="maintage">
        <div class="tage_outside">
            <div class="tage_inside">
                <div class="tage_inside_box">
                    <div class="tage_title">
                        <p>轻起来业务优势</p>
                    </div>
                    <div class="tage_detailed">
                        <ul>
                            <li>
                                <div class="detailed_title title_1">
                                    <p>一站式服务</p>
                                </div>
                                <p>公司提供涵盖商业模式策划、技术开发、运营支持及资产增值的一站式服务，真正为企业主实现增值减负。</p>
                            </li>
                            <li>
                                <div class="detailed_title title_2">
                                    <p>行业经验丰富</p>
                                </div>
                                <p>轻起来集团成立自今，经过数年的探索实践，已形成多套完善的行业商业模型，是东莞最具竞争力的综合性服务商之一。</p>
                            </li>
                            <li>
                                <div class="detailed_title title_3">
                                    <p>自有技术团队</p>
                                </div>
                                <p>独立开发技术团队，技术总监曾服务于大型电信运营商、外企投行，为开发产品的易用性、安全性保驾护航。</p>
                            </li>
                            <li>
                                <div class="detailed_title title_4">
                                    <p>一对一商洽</p>
                                </div>
                                <p>公司拥有专业的客服团队，采取一对一的商务洽谈方式，为企业用户提供更高效的售前咨询、售后服务体验。</p>
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

}
</script>

<style lang="scss" scoped>
@import '../../../dependencies/sass/style.scss';

.maintage {
    width: 100%;
    position: absolute;
    top: vm(622);
    z-index: 1;
    .tage_outside {
        background: url("../../../static/images/home/youshi/youshi_background.png");
        background-position: center center;
        background-size: contain;
        .tage_inside {
            width: vm(1200);
            height: 100%;
            margin: 0 auto;
            .tage_inside_box {
                overflow: hidden;
                .tage_title {
                    text-align: center;
                    font-size: 26px;
                    margin-top: vm(300);
                }
                .tage_detailed {
                    margin-top: vm(69);
                    padding-bottom: vm(112);
                    ul {
                        display: flex;
                        justify-content: space-around;
                        li {
                            width: vm(224);
                            margin-left: vm(52);
                            &:first-child {
                                margin-left: 0;
                            }
                            .title_1 {
                                background: url("../../../static/images/home/youshi/youshi_01.png")
                            }
                            .title_2 {
                                background: url("../../../static/images/home/youshi/youshi_02.png")
                            }
                            .title_3 {
                                background: url("../../../static/images/home/youshi/youshi_03.png")
                            }
                            .title_4 {
                                background: url("../../../static/images/home/youshi/youshi_04.png")
                            }
                            .detailed_title {
                                width: vm(190);
                                height: vm(110);
                                margin: 0 auto;
                                background-size: contain;
                                background-repeat: no-repeat;
                                padding-bottom: vm(30);
                                p {
                                    color: #fff;
                                    text-align: center;
                                    font-size: vm(22);
                                    padding-top: vm(72);
                                }
                            }
                            p {
                                font-size: vm(16);
                            }
                        }
                    }
                }
            }
        }
    }
}

</style>

