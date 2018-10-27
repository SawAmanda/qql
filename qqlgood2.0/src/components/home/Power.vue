<!-- 首页 实力组件 -->
<template>
    <section class="power">
        <div class="power_outside">
            <div class="power_inside">
                <div class="power_inside_content">
                    <div class="index_common_title power_title">
                        <p> {{power_text.title}} </p>
                    </div>
                    <div class="index_common_introduce power_introduce">
                        <p v-for="powerText in power_text.content"> {{powerText.text}} </p>
                    </div>
                    <div class="power_good">
                        <ul>
                            <li v-for="good in power_good1">
                                <div class="good_logotitle">
                                    <div class="good_logo">
                                        <img :src="good.goodURL" alt="">
                                    </div>
                                    <div class="good_title">
                                        <p>{{good.goodtitle}}</p>
                                    </div>
                                </div>
                                <div class="good_introduce">
                                    <p>{{good.goodduce}}</p>
                                </div>
                            </li>
                        </ul>
                        <ul>
                            <li v-for="good in power_good2">
                                <div class="good_logotitle">
                                    <div class="good_logo">
                                        <img :src="good.goodURL" alt="">
                                    </div>
                                    <div class="good_title">
                                        <p>{{good.goodtitle}}</p>
                                    </div>
                                </div>
                                <div class="good_introduce">
                                    <p>{{good.goodduce}}</p>
                                </div>
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
      power_text: {
        title: "为1300+企业服务的运维实力",
        content: [
          {
            text:
              "轻起来是一家专业的企业项目综合服务商，拥有多行业的项目运维经验，"
          },
          {
            text:
              "轻起来结合企业所在的行业特点，深度分析适合项目的市场营销与运营方式。"
          },
          {
            text:
              "多名专业商业古文、营销古文、社区顾问，以及丰富的行业渠道资源，能够为项目运维效果提供效益最大化的保障。"
          }
        ]
      },
      power_good1: [
        {
          goodURL: './static/images/home/yunwei/yunwei_01.png',
          goodtitle: "城市O2O",
          goodduce: "建立智能化营销体系打造品牌壁垒"
        },
        {
          goodURL: './static/images/home/yunwei/yunwei_02.png',
          goodtitle: "链接门店",
          goodduce: "将门店数字化运营提升品牌竞争力"
        },
        {
          goodURL: './static/images/home/yunwei/yunwei_03.png',
          goodtitle: "农村商贸",
          goodduce: "搭建社交互动营销机制构建O2O消费圈"
        }
      ],
      power_good2: [
        {
          goodURL: './static/images/home/yunwei/yunwei_04.png',
          goodtitle: "零售电商",
          goodduce: "打造引流-转化-沉淀自循环生态降低营销成本"
        },
        {
          goodURL: './static/images/home/yunwei/yunwei_05.png',
          goodtitle: "贸易批发",
          goodduce: "提高销量、分销管理等难题协助解决渠道规划"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "../../../dependencies/sass/style.scss";

.power {
  width: 100%;
  .power_outside {
    .power_inside {
      width: 100%;
      height: 100%;
      .power_inside_content {
        width: vm(1200);
        margin: 0 auto;
        .power_title p {
          color: #113443;
          letter-spacing: vm(1);
        }
        .power_introduce p {
          color: #768791;
        }
        .power_good {
          padding-bottom: vm(94);
          ul {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            li {
              width: vm(146);
              height: vm(200);
              margin-left: vm(254);
              &:nth-child(1) {
                margin-left: 0;
              }
              .good_logotitle {
                width: 100%;
                height: vm(109);
                .good_logo {
                  width: vm(96);
                  height: vm(65);
                  margin: 0 auto;
                }
                .good_title p {
                  font-size: vm(24);
                  letter-spacing: vm(1);
                  text-align: center;
                  background: linear-gradient(105deg, #4dc4d0, #3497dc);
                  -webkit-background-clip: text;
                  color: transparent;
                }
              }
              .good_introduce {
                font-size: vm(16);
                color: #768791;
                text-align: center;
              }
            }
          }
        }
      }
    }
  }
}
</style>
