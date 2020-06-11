<template>
	<div class="electronics">
		<div class="container">
			<h3>إلكترونيات</h3>
			<hr>
			<div class="row justify-content-around">
				<div class="col-md">
					<div class="card product" style="width: 18rem;">
						<div class="product-img">
							<img src="../../assets/imgs/headphone.png" class="card-img-top" alt="headphone">
						</div>
						<div class="card-body">
							<p class="title">سماعات</p>
						</div>
					</div>
				</div>
				<div class="col-md">
					<div class="card product" style="width: 18rem;">
						<div class="product-img">
							<img src="../../assets/imgs/tablet.png" class="card-img-top" alt="headphone">
						</div>
						<div class="card-body">
							<p class="title">تابليت</p>
						</div>
					</div>
				</div>
				<div class="col-md">
					<div class="card product" style="width: 18rem;">
						<div class="product-img">
							<img src="../../assets/imgs/laptop.png" class="card-img-top" alt="headphone">
						</div>
						<div class="card-body">
							<p class="title">لابتوب</p>
						</div>
					</div>
				</div>
				<div class="col-md">
					<div class="card product" style="width: 18rem;">
						<div class="product-img">
							<img src="../../assets/imgs/iphone.png" class="card-img-top" alt="headphone">
						</div>
						<div class="card-body">
							<p class="title">جوالات</p>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "Electronics"
}
</script>

<style lang="scss" scoped>
.electronics {
	width: 100%; height: auto;
	text-align: end;
	padding-right: 15px;
	padding-top: 15px;
	.product {
		width: unset !important;
		margin: 15px 0;
		.product-img {
			height: 120px;
			position: relative;
			display: flex;
			justify-content: center;
			align-items: center;
			background: #F7F6FC;
			cursor: pointer;
			img {
				position: relative;
				width: 60%;
				height: 85%;
				object-fit: contain;
			}
		}
		.card-body {
			text-align: center;
			width: 100%;
			height: 40px;
			line-height: 0;
			background: #333;
			color: #eee;
		}
		&:hover {
			.card-body {
				background: linear-gradient(180deg, #bd1144 25%, #4a2e76 100%, #f6fefd 100%);
			}
		}
	}
}
</style>