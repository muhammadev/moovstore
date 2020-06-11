<template>
  <div class="top-header">
    <div class="container">
      <div class="row">
        <div class="left-sec col-12 col-xl-5">
          <div class="text-holder">
            <div class="header-link">
              <a href="#">تسجيل</a>
            </div>
            <div class="header-link">
              <a href="#">تسجيل الدخول</a>
            </div>
            <div class="header-link">
              <a href="#">البيع علي منصة موف ستور</a>
            </div>
            <div class="header-link lang">
              <a href="#">EN</a>
            </div>
          </div>
        </div>
        <div class="right-sec col-12 col-xl-7">
          <div class="text-holder">
            <div class="header-link">
              <a href="#">الأقسام</a>
            </div>
            <div class="header-link">
              <a href="#">المتاجر</a>
            </div>
            <div class="header-link">
              <a href="#">اتصل بنا</a>
            </div>
            <div class="header-link">
              <a href="#">سحب موف</a>
            </div>
            <div class="header-link">
              <a href="#">سياسة الاستخدام والخصوصية</a>
            </div>
            <div class="header-link">
              <a href="#">العروض</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TopHeader",
};
</script>

<style lang="scss" scoped>
.top-header {
  border-bottom: 1px solid #eee;
  .text-holder {
    float: right;
    div {
      padding: 10px;
      line-height: 2;
      float: right;
    }
  }
  .right-sec {
    min-width: 700px;
  }
  .left-sec {
    min-width: 500px;
    .text-holder {
      float: left;
    }
  }
}

@media screen and (min-width: 1200px) {
  .container {
    max-width: 95%;
  }
}

@media screen and (max-width: 1199px) {
  .text-holder {
    float: unset !important;
    display: flex;
    justify-content: center;
  }
}
</style>
