<template>
	<div class="best-seller">
		<div class="container">
			<h3>الأكثر مبيعاً</h3>
			<hr>
			<div class="row justify-content-around">
				<div class="col-md">
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
				<div class="col-md">
					<div class="card product" style="width: 18rem;">
						<span class="new">جديد</span>
						<div class="product-img">
							<img src="../../assets/imgs/printer.png" class="card-img-top" alt="printer">
						</div>
						<div class="card-body">
								<p class="card-text">عنوان المنتج يعرض هنا</p>
								<p class="price">ريال 250.00</p>
						</div>
					</div>
				</div>
				<div class="col-md">
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
				<div class="col-md">
					<div class="card product" style="width: 18rem;">
						<span class="new">جديد</span>
						<div class="product-img">
							<img src="../../assets/imgs/laptop.png" class="card-img-top" alt="laptop">
						</div>
						<div class="card-body">
								<p class="card-text">عنوان المنتج يعرض هنا</p>
								<p class="price">ريال 250.00</p>
						</div>
					</div>
				</div>
			</div>
			<div class="row justify-content-around">
				<div class="col-md">
					<div class="card product" style="width: 18rem;">
						<span class="new">جديد</span>
						<div class="product-img">
							<img src="../../assets/imgs/laptop.png" class="card-img-top" alt="laptop">
						</div>
						<div class="card-body">
								<p class="card-text">عنوان المنتج يعرض هنا</p>
								<p class="price">ريال 250.00</p>
						</div>
					</div>
				</div>
				<div class="col-md">
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
				<div class="col-md">
					<div class="card product" style="width: 18rem;">
						<span class="new">جديد</span>
						<div class="product-img">
							<img src="../../assets/imgs/printer.png" class="card-img-top" alt="printer">
						</div>
						<div class="card-body">
								<p class="card-text">عنوان المنتج يعرض هنا</p>
								<p class="price">ريال 250.00</p>
						</div>
					</div>
				</div>
				<div class="col-md">
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
			</div>
        </div>
	</div>
</template>

<script>
export default {
	name: "BestSeller"
}
</script>

<style lang="scss" scoped>
.best-seller {
	width: 100%; height: auto;
	text-align: end;
	padding-right: 15px;
	padding-top: 15px;
	margin: 35px 0 !important;
	.product {
		width: unset !important;
		height: 230px;
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
			height: 130px;
			position: relative;
			display: flex;
			justify-content: center;
			img {
				position: relative;
			    width: 60%;
			    height: 100%;
			    bottom: -15px;
			    object-fit: contain;
			    transition: .3s ease;
		    }
		}
		.card-body {
			text-align: center;
			width: 100%;
			height: 40px;
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