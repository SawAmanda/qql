<!-- 首页 专业的区块链+开发技术团队 组件 -->
<template>
    <section class="techicalteam">
        <div class="team_outside">
            <div class="team_inside">
                <div class="index_common_title">
                    <p>专业的区块链+开发技术团队</p>
                </div>
                <div class="index_common_introduce">
                    <p>轻起来技术团队以区块链+开发为定位，团队拥有多年的区块链落地应用开发经验。</p>
                    <p>已成功开发出多套兼容网页、APP、小程序、H5的区块链应用。</p>
                    <p>区块链+技术开发为传统行业进行区块链方向转型搭建了最坚实的基础，帮助企业快速找到自身行业与区块链的切入口。</p>
                </div>
                <div class="team_content">
                    <ul>
                        <li>
                            <div class="mask"></div>
                            <div class="bg">
                                <img src="../../../static/images/home/team/kaifa_01.png" alt="">
                            </div>
                            <div class="content_box">
                                <img src="../../../static/images/home/team/kaifa_icon01.png" alt="">
                            </div>
                            <div class="content_title">
                                <p class="title">积分商城</p>
                                <div class="line"></div>
                                <p class="content_text">强大的积分系统，帮助企业维系客户、创造价值。</p>
                            </div>
                        </li>
                        <li>
                            <div class="mask"></div>
                            <div class="bg">
                                <img src="../../../static/images/home/team/kaifa_02.png" alt="">
                            </div>
                            <div class="content_box">
                                <img src="../../../static/images/home/team/kaifa_icon02.png" alt="">
                            </div>
                            <div class="content_title">
                                <p class="title">产品溯源</p>
                                <div class="line"></div>
                                <p class="content_text">记录、查询产品从生产原料到销售的全过程溯源</p>
                            </div>
                        </li>
                        <li>
                            <div class="mask"></div>
                            <div class="bg">
                                <img src="../../../static/images/home/team/kaifa_03.png" alt="">
                            </div>
                            <div class="content_box">
                                <img src="../../../static/images/home/team/kaifa_icon03.png" alt="">
                            </div>
                            <div class="content_title">
                                <p class="title">合同存证</p>
                                <div class="line"></div>
                                <p class="content_text">在去中心化的服务器上永久保存合同等存证</p>
                            </div>
                        </li>
                        <li>
                            <div class="mask"></div>
                            <div class="bg">
                                <img src="../../../static/images/home/team/kaifa_04.png" alt="">
                            </div>
                            <div class="content_box">
                                <img src="../../../static/images/home/team/kaifa_icon04.png" alt="">
                            </div>
                            <div class="content_title">
                                <p class="title">版权产业</p>
                                <div class="line"></div>
                                <p class="content_text">提供数字版权登记、版权监测、维权诉讼的平台。</p>
                            </div>
                        </li>
                        <li>
                            <div class="mask"></div>
                            <div class="bg">
                                <img src="../../../static/images/home/team/kaifa_05.png" alt="">
                            </div>
                            <div class="content_box">
                                <img src="../../../static/images/home/team/kaifa_icon05.png" alt="">
                            </div>
                            <div class="content_title">
                                <p class="title">更多应用</p>
                                <div class="line"></div>
                                <p class="content_text">金融、医疗、娱乐、食宿和教育、物联网......。</p>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style <style lang="scss" scoped>
@import '../../../dependencies/sass/style.scss';

.techicalteam {
    width: 100%;
    margin-top: vm(1340);
    .team_outside {
        background: url("../../../static/images/home/team/kaifa_background.png") no-repeat;
        background-size: cover;
        .team_inside {
            width: vm(1200);
            margin: 0 auto;
            .team_content {
                ul {
                    display: flex;
                    li {
                        width: vm(240);
                        height: vm(314);
                        position: relative;
                        overflow: hidden;
                        &:hover {
                            .mask {
                                opacity: 1;
                            }
                            .content_box img {
                                margin-top: vm(30);
                                opacity: 0;
                            }
                            .content_title {
                                .title {
                                    margin-top: vm(90);
                                }
                                .line {
                                    margin-top: vm(25);
                                    opacity: 1;
                                }
                                .content_text {
                                    opacity: 1;
                                }
                            }
                        }
                        .mask {
                            background: url("../../../static/images/home/team/kaifa_remove.png");
                            width: 100%;
                            height: 100%;
                            color: #fff;
                            transition: all 0.4s linear;
                            position: absolute;
                            top: 0;
                            left: 0;
                            z-index: 1;
                            opacity: 0;
                        }
                        .bg {
                            width: 100%;
                            height: 100%;
                            position: absolute;
                            top: 0;
                            left: 0;
                        }
                        .content_box {
                            width: 100%;
                            height: 100%;
                            position: absolute;
                            top: 0;
                            left: 0;
                            img {
                                width: vm(50);
                                margin: 0 auto;
                                opacity: 1;
                                margin-top: vm(110);
                                transition: all .4s cubic-bezier(.4,0,.2,1);
                            }
                        }
                        .content_title {
                            width: 100%;
                            height: 100%;
                            position: absolute;
                            top: 0;
                            left: 0;
                            color: #fff;
                            z-index: 2;
                            .title {
                                font-size: vm(24);
                                text-align: center;
                                margin-top: vm(190);
                                transition: all .4s cubic-bezier(.4,0,.2,1);
                            }
                            .line {
                                width: vm(38);
                                height: vm(4);
                                background: #fff;
                                border-radius: vm(2);
                                margin: 0 auto;
                                transition: all .4s cubic-bezier(.4,0,.2,1);
                                opacity: 0;
                            }
                            .content_text {
                                font-size: vm(16);
                                padding: 0 vm(25);
                                margin-top: vm(30);
                                transition: all .4s cubic-bezier(.4,0,.2,1);
                                opacity: 0;
                            }
                        }
                    }
                }
            }
        }
    }
}



</style>
