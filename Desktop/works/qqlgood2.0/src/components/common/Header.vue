<!-- 头部 logo和导航栏 组件 -->
<template>
  <header class="header">
    <div class="header_outside">
      <div class="header_inside">
        <div class="header_logo">
          <a href="">
            <img src="../../../static/images/common/logo.png" alt="">
          </a>
        </div>
        <div class="header_nav">
          <ul>
            <li v-for="Nav in list">
              <router-link :to="Nav.to"> {{Nav.name}} </router-link>
            </li>
          </ul>
        </div>
        <div class="clear"></div>
      </div>
    </div>  
  </header>
</template>

<script>
export default {
  data() {
    return {
      //头部Header 获取Nav.name数据
      list: [
        {
          name: '首页',
          to: '/'
        },
        {
          name: '最新活动',
          to: '/a'
        },
        {
          name: '经典案例',
          to: '/b'
        },
        {
          name: '产品中心',
          to: '/c'
        },
        {
          name: '项目孵化',
          to: '/d'
        },
        {
          name: '资源俱乐部',
          to: '/e'
        },
        {
          name: '项目营销',
          to: '/f'
        },
        {
          name: '服务收费',
          to: '/g'
        },
      ]
    }
  }
}
</script>


<style lang="scss">
@import '../../../dependencies/sass/style.scss';

.header {
  width: 100%;
  z-index: 2;
  position: absolute;
  top: 0;
  left: 0;
  .header_outside{
    background: rgba(0,0,0,0);
    border-bottom: 1px solid rgba(255, 255, 255, 0.123);
  }
  .header_inside {
    width: vm(1200);
    padding: vm(26) 0;
    margin: 0 auto;
    .header_logo {
      float: left;
      a {
        display: block;
        width: vm(196);
        height: vm(28);
      }
    }
    .header_nav {
      float: left;
      margin-left: vm(205);
      ul {
        display: flex;
        flex-wrap: nowrap;
        justify-content: space-between;
        li {
          &:hover a {
              color: #5cd7e1;
          }
          a {
            font-size: vm(18);
            color: #fff;
            font-family: 'SourceHanSansCN-Normal','Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
            padding-left: vm(30);
          }
        }
      }
    }
  }
}
</style>

