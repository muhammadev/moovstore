<template>
  <div class="main-category">
    <div class="details">
      <p>اكسسوارات</p>
      <h1>خصم % 50</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainCategory"
};
</script>

<style lang="scss" scoped>
.main-category {
	width: 100%;
	height: 360px;
	background: url("../../../assets/imgs/accesories.jpg") center/cover no-repeat;
	position: relative;
	overflow: hidden;
	cursor: pointer;
	.details {
		position: absolute;
		width: 100%; height: 150px;
		bottom: 0;
		background: rgba(255, 255, 255, 0.9);
		text-align: end;
		padding: 15px;
		transition: .3s ease;
		display: flex;
		flex-direction: column;
		justify-content: center;
		h1 {
			transition: .3s ease;
			position: relative;
			&::after {
				transition: .3s ease;
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
	}
	&:hover {
		.details {
			height: 100%;
			h1 {
				font-size: 40px;
				&::after {
					width: 100px;
				}
			}
		}
	}
}
</style>