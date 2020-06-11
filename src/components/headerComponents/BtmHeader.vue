<template>
  <div class="btm-header">
    <div class="text-holder">
      <div class="topic"><a href="#">الذهب والفضة</a></div>
      <div class="topic"><a href="#">أدوات وأجهزة طبية</a></div>
      <div class="topic"><a href="#">الصيدليات والأدوية</a></div>
      <div class="topic"><a href="#">الساعات</a></div>
      <div class="topic"><a href="#">النظارات والعدسات</a></div>
      <div class="topic"><a href="#">أزياء نسائية</a></div>
      <div class="topic"><a href="#">العطور</a></div>
      <div class="topic"><a href="#">الورود والهدايا</a></div>
      <div class="topic"><a href="#">أحذية وجوارب</a></div>
      <div class="topic"><a href="#">الحقائب</a></div>
      <div class="topic"><a href="#">القرطاسية</a></div>
      <div class="topic"><a href="#">المفارش</a></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BtmHeader"
};
</script>

<style lang="scss" scoped>
.btm-header {
  min-height: 55px;
  height: auto;
  background: #222;
  display: flex;
  justify-content: center;
  color: #eee;
  width: 100%;
  .text-holder {
    .topic {
      padding: 10px;
      line-height: 2.5;
      float: right;
      a {
        color: #eee;
        &:hover {
          color: rgb(211, 26, 118);
        }
      }
    }
  }
}
</style>
