<!-- 页脚 Footer 组件 -->
<template>
    <footer class="footer">
        <div class="footer_outside">
            <div class="footer_inside">
                <div class="footer_content">
                    <div class="footer_logo">
                        <img src="../../../static/images/common/logo.png" alt="">
                    </div>
                    <div class="footer_introduce">
                        <div class="footer_duce_1">
                            <ul>
                                <li>
                                    <p>公司介绍</p>
                                    <a href="">业务范围</a>
                                    <a href="">业务范围</a>
                                    <a href="">业务范围</a>
                                    <a href="">业务范围</a>
                                </li>
                                <li>
                                    <p>支持服务</p>
                                    <a href="">业务范围</a>
                                    <a href="">业务范围</a>
                                    <a href="">业务范围</a>
                                </li>
                            </ul>
                        </div>
                        <div class="footer_duce_2">
                            <div class="follow_us">
                                <p>关注我们</p>
                            </div>
                            <div class="wechat">
                                <div class="wechat_img">  
                                    <img src="../../../static/images/common/dingyuehao.png" alt="">
                                    <p>订阅号</p>
                                </div>
                                <div class="wechat_img">
                                    <img src="../../../static/images/common/fuwuhao.png" alt="">
                                    <p>服务号</p>
                                </div>
                            </div>
                        </div>
                        <div class="footer_duce_3">
                            <div class="footer_company">
                                <div class="company_text1">
                                    <p>400-9949519</p>
                                    <p>服务时间 09:00-18:00</p>
                                    <div class="clear"></div>
                                </div>
                                <div class="company_text2">
                                    <p>公司地址：东莞市南城区丰泰金翡丽中心17层</p>
                                    <p>业务电话：18688682414</p>
                                    <p>企业邮箱：qingqilaijituan@163.com</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="clear"></div>
                </div>
            </div>
        </div>
        <div class="copyright_outside">
            <div class="copyright_inside">
                <div class="copyright">
                    <p> {{copyright}} 
                        <a href="/"> {{copyrightUrl}} </a>
                    </p>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    data() {
        return {
            copyright: 'Copyright©2018-2028 轻起来区块链科技有限公司 版权所有',
            copyrightUrl: '粤ICP备18118098'
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../../dependencies/sass/style.scss';

.footer {
    width: 100%;
    .footer_outside {
        width: 100%;
        height: vm(378);
        background: #191919;
        .footer_inside {
            width: vm(1200);
            height: 100%;
            margin: 0 auto;
            .footer_content {
                padding-top: vm(107);
                font-size: vm(16);
                .footer_logo {
                    width: vm(196);
                    height: vm(28);
                    float: left;
                }
                .footer_introduce {
                    float:left;
                    .footer_duce_1 {
                        float:left;
                        ul li {
                            display: flex;
                            flex-direction: column;
                            margin-left: vm(37);
                            a {
                                color: #999;
                                margin-top: vm(18);
                                &:hover {
                                    color: #fff;
                                }
                            }
                            p {
                                color: #fff;
                                display: inline-block;
                                margin-bottom: vm(12);
                            }
                        }
                    }
                    .footer_duce_2 {
                        float: left;
                        margin-left: vm(40);
                        .follow_us {
                            p {
                                color: #fff;
                            }
                        }
                        .wechat {
                            display: flex;
                            justify-content: space-between;
                            .wechat_img {
                                margin: vm(21) vm(18) 0 0;
                                p {
                                    margin-top: vm(12);
                                    color: #999;
                                }
                            }
                        }
                    }
                    .footer_duce_3 {
                        float: left;
                        margin-left: vm(40);
                        .footer_company .company_text1 {
                            p {
                                &:first-child {
                                    font-size: vm(28);
                                    color: #5cbbc3;
                                    float: left;
                                }
                                &:nth-child(2) {
                                    font-size: vm(16);
                                    line-height: vm(30);
                                    color: #999;
                                    float: right;
                                    padding-top: vm(3);
                                }
                            }
                        }
                        .company_text2 p {
                            color: #fff;
                            margin-top: vm(27);
                        }
                    }
                }
            }
        }
        
    }
    .copyright_outside {
        width: 100%;
        height: vm(49);
        background: #252527;
        .copyright_inside {
            width: vm(1200);
            height: 100%;
            margin: 0 auto;
            .copyright p {
                color: #999;
                font-size: vm(16);
                text-align: center;
                line-height: vm(49);
                a {
                    color: #999;
                    padding-left: vm(15);
                    &:hover {
                        color: #fff;
                    }
                }
            }
        }
    }
}


</style>

