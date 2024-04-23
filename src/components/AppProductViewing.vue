<script>
export default{
    name: 'AppProductViewing'
}
</script>

<template>
    <section class="container-big">
        <div class="wrapper">
            <!-- scheda raccontaci-->
            <div class="one">
                <div class="bg-black padding-60">
                    <!-- testo e numero -->
                    <div class="title-number d-flex">
                        <h3 class="col-30">
                            Tell us what you have in mind
                        </h3>
                        <span>01</span>
                    </div>
                    <!-- /testo e numero -->
                    <!-- testo informativo -->
                    <div class="text-info absolute-text">
                        <span>MANUAL INGREDIENTS SELECTION</span>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sequi repellat iusto recusandae inventore sapiente veniam quas iure. Perferendis consectetur eaque soluta dolore quia ratione unde, rerum voluptas, provident ipsam aut.
                        </p>
                    </div>
                    <!-- /testo informativo -->
                </div>
            </div>
            <!-- /scheda raccontaci-->
            <!-- scheda cottura-->
            <div class="two">
                <div class="bg-black padding-60">
                    <!-- testo e numero -->
                    <div class="title-number d-flex">
                        <h3>
                            We Start Baking
                        </h3>
                        <span>02</span>
                    </div>
                    <!-- /testo e numero -->
                    <!-- testo informativo -->
                    <div class="text-info">
                        <span>SWEET & DELICIUS</span>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sequi repellat iusto recusandae inventore sapiente veniam quas iure. Perferendis consectetur eaque soluta dolore quia ratione unde, rerum voluptas, provident ipsam aut.
                        </p>
                    </div>
                    <!-- /testo informativo -->
                </div>
            </div>
            <!-- /scheda cottura-->
            <!-- scheda testo-->
            <div class="three padding-60">
                
                <!-- testo informativo -->
                <div class="text-info">
                    <span>DONT JUST TAKE OUR WORD FOR IT</span>
                    <p class="paragraph">
                        "Finally foun an alternative to the mass produced products. Something that incorporates real organic ingredients, nutrient dense wellness while promoting sustainability and activity."
                    </p>
                    <span>RACHEL COOPER, FOUNDER</span>
                </div>
                <!-- /testo informativo -->
                
            </div>
            <!-- /scheda testo-->
            <!-- scheda consegnato-->
            <div class="four">
                <div class="bg-black padding-60">
                    <!-- testo e numero -->
                    <div class="title-number d-flex">
                        <h3>
                            Delivered to your home
                        </h3>
                        <span>03</span>
                    </div>
                    <!-- /testo e numero -->
                    <!-- testo informativo -->
                    <div class="text-info">
                        <span>BAKED TO ORDER & GIFT WRAPPER</span>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sequi repellat iusto recusandae inventore sapiente veniam quas iure. Perferendis consectetur eaque soluta dolore quia ratione unde, rerum voluptas, provident ipsam aut.
                        </p>
                    </div>
                    <!-- /testo informativo -->
                </div>
            </div>
            <!-- /scheda consegnato-->
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;
.wrapper {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  grid-auto-rows: minmax(100px, auto);
  color: white;

    .one {
        grid-column: 1 / 3;
        grid-row: 1;
        background-image: url(../assets/images/bakery-process-1.jpg);
        background-size: cover;
        height: 500px;
        position: relative;
    }
    .two {
        grid-column: 1;
        grid-row: 2 / 4;
        background-image: url(../assets/images/bakery-process-2.jpg);
        background-size: cover;
        height: 500px;
        position: relative;
    }
    .three {
        grid-column: 2;
        grid-row: 2 / 4;
        background-color: #f2eef4;
        height: 500px;
    }
    .four {
        grid-column: 1 / 3;
        grid-row: 4;
        background-image: url(../assets/images/bakery-process-3.jpg);
        background-size: cover;
        height: 500px;
        position: relative;
    }

    .title-number{
        justify-content: space-between;
        align-items: center;

        h3{
            font-size: 30px;
        }
        span{
            font-size: 60px;
            font-family: "Poppins", sans-serif;
            font-weight: 100;
        }
    }
}

// UTILITY
.bg-black{
    position: absolute;
    background-color: rgba(0, 0, 0, 0.6);
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
}

.padding-60{
    padding: 60px;
}

.col-30{
    width: 30%;
}

.absolute-text{
    width: 30%;
    position: absolute;
    bottom: 50px; 
    right: 55px;
}

.text-info{
    

    span{
        font-size: 10px;
        font-family: "Poppins", sans-serif;
        color: #958e9b;
    }
    p{
        font-size: 14px;
        font-family: "Poppins", sans-serif;
        margin-top: 9px;
    }
    .paragraph{
        color: $color-primary;
        font-family: "Libre Baskerville", serif;
        font-weight: 600;
        font-size: 33px;
        margin: 20px 0;

    }
}



.debug{
    border: 1px dashed black;
}

</style>