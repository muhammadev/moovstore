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
  //min-height: 70px;
  padding: 10px 0;
  background: #222;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #eee;
  .text-holder {
    width: 100%;
    overflow: auto;
    white-space: nowrap;
    .topic {
      min-width: 50px;
      display: inline-block;
      line-height: 2.5;
      margin: 0 10px;
      //float: right;
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
