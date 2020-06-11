<template>
  <div class="main-offer">
  	<div class="container">
	  	<div class="row">
		  	<div class="product-img col-6">
		  		<img src="@/assets/imgs/iphonex.png" alt="" />
		  	</div>
		  	<div class="product-details col-6">
		  		<h1>IPhone <strong>X</strong></h1>
		  		<h5>احصل عليه الآن بخصم يصل إلي <strong>%20</strong></h5>
		  		<button class="btn btn-default">تسوق الآن</button>
		  	</div>
	  	</div>
  	</div>
  </div>
</template>

<script>
export default {
	name: "MainOffer"
};
</script>

<style lang="scss" scoped>
.main-offer {
	height: 400px;
	background: #f7f6fc;
	border-bottom: 1px solid #ccc;
	.container {
		height: 100%;	
		.row {
			height: 100%;
			align-items: center;
			.product-img {
				text-align: end;
			}
			.product-details {
				text-align: center;
				h1 {
					font-size: 50px;
					font-weight: lighter;
					position: relative;
					strong {
					font-weight: bold;
					}
					&::after {
						content: "";
						position: absolute;
						width: 50px;
						height: 5px;
						background: #d2136d;
						bottom: -10px;
						left: 45%;
					}
				}
				h5 {
					margin: 20px 0;
					strong {
						color: #d2136d;
					}
				}
				button {
					background: linear-gradient(180deg, #4a2e76, #bd1144 100%, #f6fefd 100%);
					color: #eee;
					font-size: 20px;
					border-radius: unset;
					&:focus {
						box-shadow: none;
					}
				}
			}
		}
	}
}
</style>