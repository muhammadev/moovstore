<template>
  <div class="top-header special-header">
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
          <div class="menu-icon">القائمة</div>
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
    //min-width: 700px;
    .menu-icon {
      display: none;
    }
  }
  .left-sec {
    //min-width: 500px;
    .text-holder {
      float: left;
    }
  }
}

@media screen and (max-width: 1199px) {
  .right-sec {
    text-align: center;
    .text-holder {
      display: inline-block;
      float: unset !important;
    }
  }
  .left-sec {
    text-align: center;
    .text-holder {
      display: inline-block;
      float: unset !important;
    }
  }
}

@media screen and (max-width: 768px) {
  .special-header {
    max-width: 100%;
    .container {
      .row {
        .left-sec {
          padding: 0 !important;
          padding-top: 5px !important;
        }
        .right-sec {
          min-width: unset !important;
          height: auto;
          * {
            float: unset;
          }
          .menu-icon {
            display: block;
            background: #eee;
            text-align: end;
            padding: 10px;
            position: relative;
            &::before {
              content: "\f107";
              position: relative;
              font-family: "fontawesome";
              left: -5px;
              color: #666;
              line-height: 2.3;
              top: 2px;
            }
          }
          .text-holder {
            height: auto;
            display: block;
            & > * {
              width: auto; height: 30px;
              margin: 15px 0;
              display: block;
              background: #eee;
              line-height: 1;
              text-align: end;
            }
          }
        }
      }
    }
  }
  .text-holder {
    * {
      font-size: 13px;
    }
  }
}

</style>
