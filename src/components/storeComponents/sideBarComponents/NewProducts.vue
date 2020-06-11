<template>
	<div class="new-products">
		<h3>أحدث المنتجات</h3>
		<hr>
		<div class="card product">
			<div class="row no-gutters">
				<div class="col-8 product-details">
					<div class="card-body">
						<p class="product-name">عنوان المنتج يعرض هنا</p>
						<p class="card-text price">ريال 250.00</p>
					</div>
				</div>
				<div class="col product-img">
					<img src="../../../assets/imgs/iron.png" class="iron" alt="iron">
				</div>
			</div>
		</div>
		<div class="card product">
			<div class="row no-gutters">
				<div class="col-8 product-details">
					<div class="card-body">
						<p class="product-name">عنوان المنتج يعرض هنا</p>
						<p class="card-text price">ريال 250.00</p>
					</div>
				</div>
				<div class="col product-img">
					<img src="../../../assets/imgs/iphone.png" class="iron" alt="iron">
				</div>
			</div>
		</div>
		<div class="card product">
			<div class="row no-gutters">
				<div class="col-8 product-details">
					<div class="card-body">
						<p class="product-name">عنوان المنتج يعرض هنا</p>
						<p class="card-text price">ريال 250.00</p>
					</div>
				</div>
				<div class="col product-img">
					<img src="../../../assets/imgs/headphone.png" class="iron" alt="iron">
				</div>
			</div>
		</div>
		<div class="card product">
			<div class="row no-gutters">
				<div class="col-8 product-details">
					<div class="card-body">
						<p class="product-name">عنوان المنتج يعرض هنا</p>
						<p class="card-text price">ريال 250.00</p>
					</div>
				</div>
				<div class="col product-img">
					<img src="../../../assets/imgs/laptop.png" class="iron" alt="iron">
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
    name: "NewProducts"
}
</script>

<style lang="scss" scoped>
.new-products {
    width: 100%;
    background: #fff;
		position: relative;
		h3 {
			text-align: end;
			position: relative;
			&::after {
				content: "";
				position: absolute;
				display: block;
				width: 70px;
				height: 8px;
				background: #333;
				right: 0;
				bottom: -20px;
			}
		}
		.product {
			position: relative;
	    width: 100%;
  	  height: 120px;
			margin: 20px 0;
			.row {
				position: absolute;
				width: 100%; height: 100%;
				.product-details {
					display: flex;
					align-items: center;
					.card-body {
						text-align: end;
						.price {
							color: #d2136d;
            }
					}
				}
				.product-img {
					height: auto;
					display: flex;
					align-items: center;
					justify-content: center;
					img {
						position: absolute;
						width: 100px;
						
					}
				}
			}
		}
}
</style>