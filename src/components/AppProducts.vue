<script>
export default{
    name: 'AppProducts',
    data() {
        return {
            isHoverVisible: false
        };
    }
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
        <div class="img-info sx" @mouseenter="isHoverVisible = true" @mouseleave="isHoverVisible = false">
            <img src="../assets/images/choco-chip-cookies-600x765.jpg" alt="">
            <div class="arrow sx d-flex">
                <i class="fa-solid fa-chevron-left"></i>
            </div>
            <div class="hover" v-if="isHoverVisible">
                <h5>Choco Chip Cookies</h5>
                <span>Cookies, Pastries</span>
                <span class="cost">$19.00 $39.00</span>
            </div>
        </div>
        <!-- /immagine sinistra -->
        <!-- immagine destra -->
        <div class="img-info dx" @mouseenter="isHoverVisible = true" @mouseleave="isHoverVisible = false">
            <img src="../assets/images/strawberry-jam-cookies-600x765.jpg" alt="">
            <div class="arrow dx d-flex">
                <i class="fa-solid fa-chevron-right"></i>
            </div>
            <div class="hover" v-if="isHoverVisible">
                <h5>Strawberry Jam Cookies</h5>
                <span>Cookies, Pastries</span>
                <span class="cost">$24.00 $62.00</span>
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

            &:hover{
                background-color: #f2eef4;
                color: $color-primary;
            }
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

        .hover {
            position: absolute;
            top: 0;
            left: 0;
            bottom: 0;
            right: 0;
            background-color: rgba(0, 0, 0, 0.4);
            color: white;
            font-size: 18px;
            display: none;
        }

        &:hover .hover {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;

            h5{
                font-size: 20px;
                margin-bottom: 8px;
            }
            span{
                font-family: "Poppins", sans-serif;
                font-size: 12px;
            }
            .cost{
                font-size: 20px;
                margin-top: 18px;
            }
        }
    }
}
</style>