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
    </header>

</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;

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


</style>