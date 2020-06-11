<template>
	<div class="side-bar">
		<MainCategory />
		<TodayDeals />
		<NewProducts />
	</div>
</template>

<script>
import MainCategory from "./sideBarComponents/MainCategory";
import TodayDeals from "./sideBarComponents/TodayDeals";
import NewProducts from "./sideBarComponents/NewProducts";

export default {
	name: "SideBar",
	components: {
		MainCategory,
		TodayDeals,
		NewProducts
	}
}
</script>

<style lang="scss" scoped>
.side-bar {
	width: 100%;
	height: 100%;
	background: #fff;
}
</style>