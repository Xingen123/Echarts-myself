<template>
  <div :class="partFive">
    <h3 class="text-center text-top">工作经验</h3>
    <p>
      <a href="javascript:void(0)">上海力沃健身管理有限公司</a>
      <span class="text-small">| 2019/03 - 至今</span>
    </p>
    <p class="text-small">工作内容：React + Antd + Redux后台管理系统、微信小程序、Vue +Iview前台管理系统……</p>
    <p class="text-small">项目成就：</p>
    <p class="text-small">&emsp;1. 使用原生代码进行微信小程序的开发。</p>
    <p class="text-small">&emsp;2. 使用 Vue + Iview + Vuex开发前台系统,React + Antd + Redux开发后台管理系统</p>
    <p class="text-small">&emsp;3. Vue + Vant开发客户端移动项目。</p>
    <br />
    <br />
    <p>
      <a href="javascript:void(0)">北京悦活餐饮管理有限责任公司</a>
      <span class="text-small">| 2017/03 - 2019/02</span>
    </p>
    <p class="text-small">工作内容：jQuery活动页,微信小程序、Vue + Element后台管理系统……</p>
    <p class="text-small">项目成就：</p>
    <p class="text-small">&emsp;1. 官网搭建，后台系统的开发。</p>
    <p class="text-small">&emsp;2. 使用 Vue + Element开发后台管理系统，进行商品的管理。</p>
    <p class="text-small">&emsp;3. jQuery 活动页及 H5 活动页。</p>
  </div>
</template>

<script>
export default {
  name: "partFive",
  data () {
    return {
      partFive: "part-five",
      curWidth: 0
    };
  },
  beforeMount () {
    this.curWidth = document.documentElement.clientWidth || document.body.clientWidth;
    if (this.curWidth < 1600) {
      this.partFive = "part-five-responsive"
    }
  }
};
</script>

<style scoped>
a {
  color: deepskyblue;
}
a:hover {
  color: rgb(118, 190, 248);
}
.part-five {
  width: 100%;
  height: 310px;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
}
.part-five-responsive {
  width: 100%;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
}
.text-center {
  text-align: center;
}
.text-small {
  font-size: 0.9em;
  color: rgb(253, 239, 239);
}
</style>