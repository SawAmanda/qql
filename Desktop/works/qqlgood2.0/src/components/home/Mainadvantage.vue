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
                                    <p>一站式服务</p>
                                </div>
                                <p>公司提供涵盖商业模式策划、技术开发、运营支持及资产增值的一站式服务，真正为企业主实现增值减负。</p>
                            </li>
                            <li>
                                <div class="detailed_title title_3">
                                    <p>一站式服务</p>
                                </div>
                                <p>公司提供涵盖商业模式策划、技术开发、运营支持及资产增值的一站式服务，真正为企业主实现增值减负。</p>
                            </li>
                            <li>
                                <div class="detailed_title title_4">
                                    <p>一站式服务</p>
                                </div>
                                <p>公司提供涵盖商业模式策划、技术开发、运营支持及资产增值的一站式服务，真正为企业主实现增值减负。</p>
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
        height: vm(750);
        background: url("../../../static/images/home/youshi/youshi_background.png");
        background-position: center center;
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
                    ul {
                        display: flex;
                        justify-content: space-around;
                        li {
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

