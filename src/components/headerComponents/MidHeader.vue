<template>
  <div class="mid-header">
    <div class="row align-items-center">
      <div class="shoping-cart col-xl-2 order-3 order-xl-1">
        <i class="fas fa-shopping-cart"></i>
        <a href="#">عربة التسوق</a>
      </div>
      <div class="search col-xl-7 order-2">
        <button type="submit" class="btn btn-search">
          <i class="fas fa-search"></i>
        </button>
        <input
          class="search-field"
          type="text"
          placeholder="ابحث في الأقسام الخاصة بنا"
          required
        />
        <a href="#">
          <div class="menu">
            جميع الفئات
          </div>
        </a>
      </div>
      <div class="logo col-xl-3 order-1 order-xl-3">
        <img src="@/assets/imgs/moov_sticky.webp" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MidHeader",
};
</script>

<style lang="scss" scoped>
.mid-header {
  min-height: 100px;
  margin-top: 30px;
  .row {
    height: 100%;
    .shoping-cart {
      text-align: center;
      a {
        margin-left: 5px;
      }
    }
    .search {
      text-align: center;
      position: relative;
      border: 1px solid #ccc;
      height: 40px;
      display: flex;
      padding: 0;
      * {
        height: 100%;
      }
      .menu {
        position: relative;
        //display: inline-block;
        width: 15%;
        min-width: 120px;
        flex-grow: 1;
        font-size: 15px;
        text-align: end;
        padding-right: 10px;
        right: 0;
        &::before {
          content: "\f107";
          position: relative;
          font-family: "fontawesome";
          right: 5px;
          color: #666;
          line-height: 2.3;
          top: 2px;
        }
        &::after {
          content: "";
          position: absolute;
          left: 0px;
          height: 25px;
          width: 1px;
          background: #ccc;
          top: calc(50% - 12.5px);
        }
      }
      .search-field {
        //position: absolute;
        min-width: 130px;
        flex-grow: 2;
        //right: 15%;
        text-align: end;
        outline: none;
        border: none;
        padding-right: 10px;
      }
      .btn-search {
        //position: absolute;
        //left: 0;
        min-width: 40px;
        flex-grow: 0.1;
        border: none;
        border-radius: 0;
        line-height: 2;
        color: #eee;
        background: linear-gradient(180deg, rgba(189,17,68,1) 25%, rgba(74,46,118,1) 100%, rgba(246,254,253,1) 100%);
        /*&::after {
          content: "";
          position: absolute;
          top: 33%;
          right: -20px;
          width: 20px;
          border: medium solid #4a2e76;
          border-width: 5px 0px 5px 5px;
          border-color: transparent transparent transparent #4a2e76;
        }*/
      }
    }
    .logo {
      text-align: center;
      img {
        height: 70px;
      }
    }
  }
}

@media screen and (max-width: 1199px) {
  .mid-header {
    margin-top: 0 !important;
    .row {
      max-width: 95%;
      margin: auto;
      & > * {
        margin: 30px 0;
      }
    }
  }
}

@media screen and (max-width: 768px) {
  .search-field {
    font-size: 13px !important;
  }
  .menu {
    min-width: 100px !important;
    font-size: 13px !important;
    line-height: 3;
  }
}
</style>
