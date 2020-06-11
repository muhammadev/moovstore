<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col col-xl-3 order-5">
          <h3>نبذة عنا</h3>
					<div class="text-holder">
						<p class="about"> لوريم ايبسوم هو نموذج افتراضي يوضع في التصاميم لتعرض على العميل ليتصور طريقه وضع النصوص بالتصاميم سواء كانت تصاميم مطبوعه</p>
						<div class="tel">
							<a href="tel:966-195745 5814 99452">966-195745 5814 99452 | 966-714522 4215 42157</a>
							<i class="fas fa-phone-alt"></i>
						</div>
						<div class="mail">
							<a href="mailto:Admin@domainname.com">Admin@domainname.com</a>
							<i class="far fa-envelope"></i>
						</div>
						<div class="social-media">
							<p class="facebook">
								<i class="fab fa-facebook-f"></i>
							</p>
							<p class="twitter">
								<i class="fab fa-twitter"></i>
							</p>
							<p class="instagram">
								<i class="fab fa-instagram"></i>
							</p>
							<p class="snapchat">
								<i class="fab fa-snapchat-ghost"></i>
							</p>
					</div>
          </div>
        </div>
        <div class="col order-4">
					<h3>الأقسام</h3>
					<ul>
						<a href="#"><li>من نحن</li></a>
						<a href="#"><li>منتجاتنا</li></a>
						<a href="#"><li>العلامات التجارية</li></a>
						<a href="#"><li>الشركات التابعة</li></a>
						<a href="#"><li>العروض الخاصة</li></a>
						<a href="#"><li>أسئلة وأجوبة</li></a>
					</ul>
        </div>
        <div class="col order-3">
					<h3>الحساب الشخصي</h3>
					<ul>
						<a href="#"><li>من نحن</li></a>
						<a href="#"><li>منتجاتنا</li></a>
						<a href="#"><li>العلامات التجارية</li></a>
						<a href="#"><li>الشركات التابعة</li></a>
						<a href="#"><li>العروض الخاصة</li></a>
						<a href="#"><li>أسئلة وأجوبة</li></a>
					</ul>
        </div>
        <div class="col order-2">
					<h3>معلومات</h3>
					<ul>
						<a href="#"><li>من نحن</li></a>
						<a href="#"><li>منتجاتنا</li></a>
						<a href="#"><li>العلامات التجارية</li></a>
						<a href="#"><li>الشركات التابعة</li></a>
						<a href="#"><li>العروض الخاصة</li></a>
						<a href="#"><li>أسئلة وأجوبة</li></a>
					</ul>
        </div>
        <div class="col order-1">
            <h3>لتحميل التطبيق</h3>
						<div class="app-badges">
							<img src="@/assets/imgs/appstore.png" alt="" />
							<img src="@/assets/imgs/googleplay.png" alt="" />
						</div>
        </div>
      </div>
			<hr>
			<p class="copywrite"> &copy; جميع الحقوق محفوظة لموف ستور ٢٠٢٠</p>
    </div>
  </footer>
</template>

<script>
export default {
	name: "Footer"
}
</script>

<style lang="scss" scoped>
footer{
	margin-top: 50px;
	padding: 50px;
	padding-bottom: 10px;
	background: #333;
	color: #eee;
	text-align: end;
	h3 {
		font-size: 20px !important;
		&::after {
			background: #d2136d !important;
		}
	}
	.text-holder {
		margin-top: 70px;
		.about {
			font-size: 15px;
		}
		.tel,.mail {
			font-size: 12px;
			display: flex;
			justify-content: flex-end;
			margin: 15px 0;
			a {
				margin-right: 15px;
			}
		}
	}
	ul {
		margin-top: 70px;
		li {
			margin: 10px 0;
		}
	}
	a {
		color: #eee;
	}
	.social-media {
		& > * {
			margin-left: 15px;
			width: 30px;
			height: 30px;
			background: #eee;
			color: #333;
			text-align: center;
			line-height: 2.5;
			float: right;
			cursor: pointer;
			&:hover {
				color: #eee;
			}
		}
		.facebook:hover {
			background:  #3b5998;
		}
		.twitter:hover {
			background:  #00aced;
		}
		.instagram:hover {
			background: #E1306C;
		}
		.snapchat:hover {
			background: #fffc00;
		}
	}
	.app-badges {
		height: 100%;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-end;
		& > img {
			width: 150px;
			margin: 10px 0;
			cursor: pointer;
		}
	}
	.copywrite {
		text-align: center;
	}
}
</style>