<script>
export default{
    name: 'AppHeader',
}
</script>

<template>

    <header>
        <section class="nav-bar">
            <div class="container d-flex">
                <!-- logo -->
                <img src="../assets/images/avada-bakery-logo.png" alt="">
                <!-- /logo -->
                <!-- menu nav-bar -->
                <nav>
                    <ul class="d-flex">
                        <li>Home</li>
                        <li>Home</li>
                        <li>Home</li>
                        <li>Home</li>
                        <li><i class="fa-solid fa-cart-shopping"></i></li>
                    </ul>
                </nav>
                <!-- /menu nav-bar -->
            </div>
        </section>
        <!-- info-sections -->
        <div class="info-hero">
            <span>FRESH & TASTY BAKERY EVERY DAY</span>
            <h2>
                The Perfect Fresh Bread
            </h2>
            <p>
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quam quia tenetur autem alias accusantium laboriosam ut exerci
            </p>
            <button class="btn">Explore our products</button>
        </div>
        <!-- info-sections -->
    </header>

</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;
header{
    min-height: 500px;
    background-image: url(../assets/images/hero-header-bakery.jpg);
    background-position: 10% 50%;
    background-size: cover;
    position: relative;
}

.nav-bar{
    padding: 15px;

    .container{
        align-items: center;
        justify-content: space-between;

        img{
            height: 45px;
        }

        ul{
            font-family: "Poppins", sans-serif;

            li{
                color: $color-primary;
                margin: 0 10px;

                i{
                    font-size: 12px;
                }
            }
        }
    }
}
.info-hero{
    padding: 30px;
    width: 35%;
    margin: 30px 20px;

    span{
        font-family: "Poppins", sans-serif;
        font-size: 9px;
        color: #958e9b;
    }
    h2{
        color: $color-primary;
        font-size: 30px;
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
        color: $color-primary;
    }
}


</style>