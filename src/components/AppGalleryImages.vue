<script>
export default{
    name: 'AppGalleryImages'
}
</script>

<template>
    <section class="container-big social">
        <div class="wrapper">
            <div class="one">
                <img src="../assets/images/social-1.jpg" alt="">
            </div>
            <div class="two">
                <!-- testo informativo -->
                <div class="text-info d-flex">
                    <span>MADE FOR SHARING</span>
                    <h4>
                        Let's stay in touch
                    </h4>
                    <button class="btn"><i class="fa-brands fa-instagram"></i>Follow Us</button>
                </div>
                <!-- /testo informativo -->
            </div>
            <div class="three">
                <img src="../assets/images/social-2.jpg" alt="">
            </div>
            <div class="four">
                <img src="../assets/images/social-3.jpg" alt="">
            </div>
            <div class="five">
                <img src="../assets/images/social-5.jpg" alt="">
            </div>
            <div class="six">
                <img src="../assets/images/social-4.jpg" alt="">
            </div>
            <div class="seven">
                <img src="../assets/images/social-6.jpg" alt="">
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;
.social{
    margin-top: 110px;
}
.wrapper {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
  grid-auto-rows: minmax(100px, auto);

    .one {
        grid-column: 1 / 2;
        grid-row: 1 / 3;
    }
    .two {
        grid-column: 2 / 4;
        grid-row: 1 / 3;
    }
    .three {
        grid-column: 4 / 5;
        grid-row: 1 / 3;
    }
    .four {
        grid-column: 1 / 2;
        grid-row: 3 / 5;
    }
    .five {
        grid-column: 2 / 3;
        grid-row: 3 / 5;
    }
    .six {
        grid-column: 3 / 4;
        grid-row: 3 / 5;
    }
    .seven {
        grid-column: 4 / 5;
        grid-row: 3 / 5;
    }
}

.text-info{
    height: 100%;
    background-color: #f2eef4;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    
    span{
        font-size: 10px;
        font-family: "Poppins", sans-serif;
        color: #958e9b;
    }
    h4{
        color: $color-primary;
        font-weight: 800;
        font-size: 20px;
        margin: 10px 0;
    }
    button{
        color: white;
        background-color: $bg-primary;

        i{
            margin-right: 7px;
        }
    }
}

// UTILITY
img{
    display: block;
}

.debug{
    border: 1px dashed black;
}

</style>