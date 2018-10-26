<!-- 首页 孵化平台 组件 -->

<template>
    <section class="platform">
        <div class="platform_outside">
            <img src="../../../static/images/home/touzi_background.png" alt="">
            <div class="platform_inside">
                <div class="platform_inside_content">
                    <div class="index_common_title">
                        <p>全球创业者的加速孵化平台</p>
                    </div>
                    <div class="index_common_introduce">
                        <p>轻起来依托雄厚的产业资源、渠道资源，为光大创业者提供创业孵化土壤，实现合作与投资的系统结合。</p>
                        <p>对于有潜力的合作项目，轻起来将会以注资入股或提供管理经验的方式，共同促进创业项目的发展。</p>
                    </div>
                    <div class="platform_nav">
                        <ul>
                            <li>
                                <a href="">资金投资</a>
                            </li>
                            <li>
                                <a href="">项目管理</a>
                            </li>
                            <li>
                                <a href="">渠道引流</a>
                            </li>
                            <li>
                                <a href="">社区搭建</a>
                            </li>
                            <div class="clear"></div>
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

.platform {
    width: 100%;
    .platform_outside {
        height: vm(440);
        position: relative;
        .platform_inside {
            width: 100%;
            height: 100%;
            position: absolute;
            top: 0;
            left: 0;
            .platform_inside_content {
                width: vm(1200);
                height: vm(440);
                margin: 0 auto;
                .platform_nav {
                    ul {
                        display: flex;
                        justify-content: space-around;
                        li {
                            margin-left: vm(60);
                            a {
                                color: #b09c5c;
                                padding: vm(17) vm(38);
                                border: 2px solid #fff;
                                background: rgba(255, 255, 255, 0);
                            }
                        }
                    }
                }
            }
        }
    }
}


</style>

