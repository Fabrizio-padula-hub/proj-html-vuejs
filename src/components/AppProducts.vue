<script>
export default{
    name: 'AppProducts'
}
</script>

<template>
    <section class="all-products d-flex container-big">
        <!-- bottone e testo -->
        <div class="info-wrapper">
            <span>OUR PRODUCTS</span>
            <h3>
                All our delectable pastries are backed fresh in our Kitchen very morning, and are made with all-natural, all organic ingredients.
            </h3>
            <button class="btn">Start Shopping</button>
        </div>
        <!-- /bottone e testo -->
        <!-- immagine sinistra -->
        <div class="img-info sx">
            <img src="../assets/images/choco-chip-cookies-600x765.jpg" alt="">
            <div class="arrow sx d-flex">
                <i class="fa-solid fa-chevron-left"></i>
            </div>
        </div>
        <!-- /immagine sinistra -->
        <!-- immagine destra -->
        <div class="img-info dx">
            <img src="../assets/images/strawberry-jam-cookies-600x765.jpg" alt="">
            <div class="arrow dx d-flex">
                <i class="fa-solid fa-chevron-right"></i>
            </div>
        </div>
        <!-- /immagine destra -->
    </section>

</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;
.all-products{
    min-height: 300px;

    .info-wrapper{
        padding-right: 40px;

        span{
            font-family: "Poppins", sans-serif;
            font-size: 9px;
            color: #958e9b;
        }
        h3{
            color: $color-primary;
            font-size: 20px;
            font-weight: 800;
            margin: 16px 0;
        }
        button{
            background-color: $bg-primary;
            color: white;
            margin-top: 20px;
        }
    }
    

    .img-info{
        width: 100%;
        object-fit: contain;
        overflow: hidden;
        position: relative;

        &.sx{
            margin: 0 10px;
        }

        .arrow{
            background-color: #a691b2;
            position: absolute;
            top: 50%;
            color: #fff;
            height: 40px;
            width: 20px;
            align-items: center;
            justify-content: center;

            &.sx{
                left: 0;
            }

            &.dx{
                right: 0;
            }

        }
    }
}
</style>