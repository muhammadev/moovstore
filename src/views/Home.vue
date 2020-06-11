<template>
  <div class="home">
    <AppHeader />
    <MainOffer />
    <MainStore />
    <MainCategories />
    <MainElectronics />
    <div class="container flags">
      <div class="row">
        <div class="col-md flag">
          <p>أفضل سعر مضمون</p>
          <i class="fas fa-ticket-alt"></i>
        </div>
        <div class="col-md flag">
          <p>دعم ٢٤ ساعة / ٧ أيام</p>
          <i class="fas fa-retweet"></i>
        </div>
        <div class="col-md flag">
          <p>دفع آمن ٪١٠٠</p>
          <i class="fab fa-cc-visa"></i>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader.vue";
import MainOffer from "@/components/MainOffer.vue";
import MainStore from "@/components/MainStore.vue";
import MainCategories from "@/components/MainCategories.vue";
import MainElectronics from "@/components/MainElectronics.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    AppHeader,
    MainOffer,
    MainStore,
    MainCategories,
    MainElectronics,
    Footer
  }
};
</script>

<style lang="scss" scoped>
.home {
  .flags {
    margin-top: 30px;
    .row {
      justify-content: space-between;
      .flag {
        padding: 20px;
        min-width: 300px; height: 80px;
        margin: 10px;
        line-height: 2;
        max-width: unset !important;
        // flex: unset !important;
        background: linear-gradient(180deg, rgba(189,17,68,1) 25%, rgba(74,46,118,1) 100%, rgba(246,254,253,1) 100%);
        color: #eee;
        text-align: center;
        font-size: 20px;
        p {
          display: inline;
          margin: 0 20px;
        }
      }
    }
  }
}
</style>
