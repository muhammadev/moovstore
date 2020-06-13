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
          <div @click="showMenu" class="menu-icon">
            <i class="fas fa-bars"></i>
          </div>
          <div class="text-holder" :class="{opened: opened}">
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
  data: function() {
    return {
      opened: false
    }
  },
  mounted() {
    this.$on("showMenu", function() {
      this.opened = !this.opened;
    })
  },
  methods: {
    showMenu() {
      this.$emit("showMenu")
    }
  }
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
          text-align: start;
          .text-holder {
            padding-right: 0px;
            .header-link {
              padding: 5px;
            }
          }
        }
        .right-sec {
          min-width: unset !important;
          height: 0;
          text-align: end;
          * {
            float: unset;
          }
          .menu-icon {
            display: inline-block;
            width: 50px;
            padding: 10px 20px;
            line-height: 2;
            position: absolute;
            top: -50px; right: -8px;
            cursor: pointer;
          }
          .text-holder {
            width: 100%; height: 0px;
            display: block;
            overflow: hidden;
            transition: .3s ease;
            background: #eee;
            margin-bottom: 10px;
            position: absolute;
            left: 0;
            z-index: 10000;
            & > * {
              width: auto; height: 30px;
              margin: 15px 0;
              display: block;
              line-height: 1;
              text-align: end;
              a {
                font-size: 15px;
              }
            }
          }
          .opened {
            height: 300px !important;
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
