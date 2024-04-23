<script>
export default{
    name: 'AppShop'
}
</script>

<template>
    <section class="container-big">
        <div class="wrapper">
            <!-- sezione testo -->
            <div class="one d-flex">
                <h3>
                    Find a freshly baked product perfect for you
                </h3>
                <p>
                    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Error delectus numquam porro unde, velit debitis repudiandae ut dolorem
                </p>
                <button class="btn">Shop All Products</button>
            </div>
            <!-- /sezione testo -->
            <!-- sezione immagini -->
            <div class="img-product two">
                <img src="../assets/images/choco-chip-cookies-200x255.jpg" alt="">
                <h5>Choco Chip Cookies</h5>
                <span>$19.00 - $39.00</span>
                <div class="arrow sx d-flex">
                    <i class="fa-solid fa-chevron-left"></i>
                </div>
            </div>
            <div class="img-product three">
                <img src="../assets/images/strawberry-jam-cookies-200x255.jpg" alt="">
                <h5>Strawberry Jam Cookies</h5>
                <span>$24.00 - $62.00</span>
            </div>
            <div class="img-product four">
                <img src="../assets/images/strawberry-donut-200x255.jpg" alt="">
                <h5>Strawberry Donut</h5>
                <span>$24.00 - $42.00</span>
            </div>
            <div class="img-product five">
                <img src="../assets/images/perfect-macarons-200x255.jpg" alt="">
                <h5>Perfect Macarons</h5>
                <span>$18.00 - $52.00</span>
                <div class="arrow dx d-flex">
                    <i class="fa-solid fa-chevron-right"></i>
                </div>
            </div>
            <!-- /sezione immagini -->
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;

.wrapper{
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    min-height: 200px;
    margin: 70px 0;

    .one{
        text-align: center;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        
        h3{
            color: $color-primary;
            font-size: 20px;
            font-weight: 800;
            margin: 16px 0;
        }
        p{
            font-family: "Poppins", sans-serif;
            font-size: 9px;
            color: #958e9b;
            margin-bottom: 16px;
        }
        button{
            background-color: $bg-primary;
            color: white;
            margin-top: 10px;
        }
    }
    .img-product{
        text-align: center;
        position: relative;
        h5{
            color: $color-primary;
            margin: 10px 0;
        }
        span{
            color: $color-primary;
            font-size: 12px;
        }
        .arrow{
            background-color: #a691b2;
            position: absolute;
            top: 40%;
            color: #fff;
            height: 40px;
            width: 20px;
            align-items: center;
            justify-content: center;

            &.sx{
                left: 30px;
            }

            &.dx{
                right: 30px;
            }

        }
    }
}
</style>