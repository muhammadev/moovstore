<template>
  <div class="main-store">
    <div class="container">
      <div class="row">
        <div class="col-lg-9 col-md-8">
					<Electronics />
					<Chosen />
					<Ads />
					<BestSeller />
				</div>
        <div class="col-lg-3 col-md-4">
          <SideBar />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SideBar from "@/components/storeComponents/SideBar.vue";
import Electronics from "@/components/storeComponents/Electronics.vue";
import Chosen from "@/components/storeComponents/Chosen.vue";
import Ads from "@/components/storeComponents/Ads.vue";
import BestSeller from "@/components/storeComponents/BestSeller.vue";

export default {
  name: "MianStore",
  components: {
		SideBar,
		Electronics,
		Chosen,
		Ads,
		BestSeller
  }
};
</script>

<style lang="scss" scoped>
.main-store {
  width: 100%;
  height: auto;
  background: #fff;
	margin-top: 30px;
  * {
	  padding: 0;
  }
  .container {
    max-width: 95%;
		height: 100%;
    .row {
			margin: auto;
      width: 100%;
      height: 100%;
			.col-9 {
				& > * {
					margin: 20px 0;
				}
			}
    }
  }
}
</style>