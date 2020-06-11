<template>
    <div class="today-deals">
        <h3>صفقات اليوم</h3>
        <hr>
        <div class="card product">
            <img src="../../../assets/imgs/screen.jpg" class="screen" alt="screen">
            <div class="card-body">
                <p class="card-text">عنوان المنتج يعرض هنا</p>
                <p class="price">ريال 250.00</p>
            </div>
            <div class="card-footer text-danger">
                منتهية الصلاحية
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "TodayDeals"
}
</script>

<style lang="scss" scoped>
.today-deals {
    width: 100%; height: 460px;
    background: #fff;
    margin-top: 30px;
    // padding: 15px;
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
        height: 350px;
        cursor: pointer;
        margin-top: 30px;
        img {
            width: 100%; height: 200px;
            object-fit: cover;
        }
        .card-body {
            text-align: center;
            font-family: bold;
            font-family: "Tajawal", sans-serif !important;
            .price {
                color: #d2136d;
            }
        }
        .card-footer {
            background: #fff !important;
            text-align: center;
        }
    }
}
</style>