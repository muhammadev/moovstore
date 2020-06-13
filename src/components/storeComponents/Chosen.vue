<template>
	<div class="chosen">
		<div class="container">
			<h3>اخترنا لك</h3>
			<hr>
			<div class="row justify-content-around">
				<div class="col-md">
					<div class="row">
						<div class="col-xl">
							<div class="card product" style="width: 18rem;">
								<span class="new">جديد</span>
								<div class="product-img">
									<img src="../../assets/imgs/headphone.png" class="card-img-top" alt="headphone">
								</div>
								<div class="card-body">
										<p class="card-text">عنوان المنتج يعرض هنا</p>
										<p class="price">ريال 250.00</p>
								</div>
							</div>
						</div>
						<div class="col-xl">
							<div class="card product" style="width: 18rem;">
								<span class="new">جديد</span>
								<div class="product-img">
									<img src="../../assets/imgs/iphone.png" class="card-img-top" alt="iphone">
								</div>
								<div class="card-body">
										<p class="card-text">عنوان المنتج يعرض هنا</p>
										<p class="price">ريال 250.00</p>
								</div>
							</div>
						</div>
					</div>
				</div>
				<div class="col-md">
					<div class="row">
						<div class="col-xl">
							<div class="card product" style="width: 18rem;">
								<span class="new">جديد</span>
								<div class="product-img">
									<img src="../../assets/imgs/tablet.png" class="card-img-top" alt="tablet">
								</div>
								<div class="card-body">
										<p class="card-text">عنوان المنتج يعرض هنا</p>
										<p class="price">ريال 250.00</p>
								</div>
							</div>
						</div>
						<div class="col-xl">
							<div class="card product" style="width: 18rem;">
								<span class="new">جديد</span>
								<div class="product-img">
									<img src="../../assets/imgs/iron.png" class="card-img-top" alt="iron">
								</div>
								<div class="card-body">
										<p class="card-text">عنوان المنتج يعرض هنا</p>
										<p class="price">ريال 250.00</p>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "Chosen"
}
</script>

<style lang="scss" scoped>
.chosen {
	width: 100%; height: auto;
	text-align: end;
	margin-top: 15px;
	.product {
		width: unset !important;
		height: auto;
		margin: 15px 0;
		span.new {
			position: absolute;
			width: 30px;
			text-align: center;
			top: 10px;
			color: #2aec6d;
			left: 10px;
			font-size: 12px;
			line-height: 2;
			&::before {
				content: "";
				position: absolute;
				width: 30px;
				height: 1px;
				background: #2aec6d;
				top: 0px;
				left: 0;
			}
			&::after {
				content: "";
				position: absolute;
				width: 30px;
				height: 1px;
				background: #2aec6d;
				bottom: 0;
				left: 0;
			}
		}
		.product-img {
			height: auto;
			padding-top: 10px;
			position: relative;
			display: flex;
			justify-content: center;
			img {
				position: relative;
			    width: 60%;
			    height: 130px;
			    bottom: -15px;
			    object-fit: contain;
			    transition: .3s ease;
		    }
		}
		.card-body {
			text-align: center;
			width: 100%;
			height: auto;
			padding: 0;
			padding-top: 20px;
			.price {
				color: #d2136d;
			}
		}
		&:hover {
			img {
				transform: scale(1.1);
			}
		}
	}
}
</style>