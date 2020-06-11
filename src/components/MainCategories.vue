<template>
	<div class="main-categos">
		<div class="container">
			<div class="row">
				<div class="col-md">
					<div class="row">
						<div class="col-lg">
							<div class="main-category">
								<div class="details">
									<p>اكسسوارات</p>
									<h1>خصم % 50</h1>
								</div>
							</div>
						</div>
						<div class="col-lg">
							<div class="main-category clothes-tools">
								<div class="details">
									<p>اكسسوارات</p>
									<h1>خصم % 50</h1>
								</div>
							</div>
						</div>
					</div>
				</div>
				<div class="col-md">
					<div class="row">
						<div class="col-lg">
							<div class="main-category leather-bag">
								<div class="details">
									<p>اكسسوارات</p>
									<h1>خصم % 50</h1>
								</div>
							</div>
						</div>
						<div class="col-lg">
							<div class="main-category clean-tools">
								<div class="details">
									<p>اكسسوارات</p>
									<h1>خصم % 50</h1>
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
  name: "MainCategories"
};
</script>

<style lang="scss" scoped>
.main-category {
	width: 100%;
	height: 360px;
	margin: 10px 0;
	background: url("../assets/imgs/accesories.jpg") center/cover no-repeat;
	position: relative;
	overflow: hidden;
	cursor: pointer;
	.details {
		position: absolute;
		width: 100%; height: 100%;
		bottom: -65%;
		background: rgba(255, 255, 255, 0.9);
		text-align: end;
		padding: 15px;
		transition: .3s ease;
		* {
			transition: .3s;
		}
		h1 {
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
				transition: .3s;
			}
		}
	}
	&:hover .details {
		bottom: 0;
		padding-top: 50%;
		h1 {
			font-size: 50px;
			&::after {
				width: 100px;
			}
		}
	}
}
.clean-tools {
	background: url("../assets/imgs/clean-tools.jpg") center/cover no-repeat;
}
.leather-bag {
	background: url("../assets/imgs/leather-bag.jpg") center/cover no-repeat;	
}
.clothes-tools {
	background: url("../assets/imgs/clothes-tools.jpg") center/cover no-repeat;	
}
</style>