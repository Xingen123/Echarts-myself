<template>
  <div class="part-one">
    <img class="part-one-image" :src="headImage" alt="头像">
    <p>姓&emsp;&emsp;名：邢恩</p>
    <p>学&emsp;&emsp;历：大专</p>
    <p>工作年限：3 年</p>
    <p>年&emsp;&emsp;龄：22</p>
    <p>联系电话：15006786952</p>
    <p>电子邮箱：335728491@qq.com</p>
    <p>掘&emsp;&emsp;金：<a href="https://juejin.im/user/5a990d7c6fb9a028ca526a83/posts" target="_blank">Let's go </a></p>
    <p>GitHub：<a href="https://github.com/Xingen123" target="_blank">Let's go </a></p>
  </div>
</template>

<script>
export default {
  name: "partOne",
  data() {
    return {
      headImage: require('../assets/img/head_image.png')
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
p {
  line-height: 30px;
}
.part-one {
  width: 100%;
  height: 500px;
  border: 40px solid transparent;
  border-image: url("~@/./assets/img/border_image.png") 30 30 stretch;
  background: #18202d;
  padding-left: 10px;
}
.part-one-image {
  width: 150px;
  height: 150px;
}
</style>