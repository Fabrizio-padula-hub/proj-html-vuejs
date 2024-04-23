<script>
export default{
    name: 'AppCityWork'
}
</script>

<template>
    <section class="container-big">
        <!-- titolo -->
        <div class="title">
            <span>LOCATIONS</span>
            <h3>Visit our Bakeries</h3>
        </div>
        <!-- /titolo -->
        <!-- sezione immagini e info -->
        <div class="store-information d-flex">
            <!-- sezione new york -->
            <div class="ny">
                <div class="presentation-img">
                   <img src="../assets/images/new-york-bk.jpg" alt="">
                </div>
                <div class="city-ny d-flex">
                    <div class="col-30 d-flex">
                        <span>CALL US</span>
                        <span>1.800.458.556</span>
                    </div>
                    <div class="col-30 d-flex">
                        <h5>New York</h5>
                        <span>OPEN ALL WEEK</span>
                        <span>9:00 AM - 6.00 PM</span>
                    </div>
                    <div class="col-30">
                        <button class="btn">View Map</button>
                    </div>
                </div>
            </div>
            <!-- /sezione new york -->
            <!-- sezione londra -->
            <div class="ldn">
                <div class="presentation-img">
                    <img src="../assets/images/london-bk.jpg" alt="">
                </div>
                <div class="city-ldn d-flex">
                    <div class="col-30 d-flex">
                        <span>CALL US</span>
                        <span>1.800.458.556</span>
                    </div>
                    <div class="col-30 d-flex">
                        <h5>London</h5>
                        <span>OPEN ALL WEEK</span>
                        <span>9:00 AM - 6.00 PM</span>
                    </div>
                    <div class="col-30">
                        <button class="btn">View Map</button>
                    </div>
                </div>
            </div>
            <!-- sezione londra -->
        </div>
        <!-- /sezione immagini e info -->
        
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;
.title{
    text-align: center;

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
}

.store-information{
    text-align: center;
    margin-top: 40px;

    .ny{
        background-color: #f1f9fb;
        img{
            object-fit: cover;
        }
    }
    .ldn{
        background-color: #faf3e3;
    }
    .city-ny,
    .city-ldn{
        align-items: flex-end;
        margin: 20px 0;
        
        h5{
            font-size: 20px;
            color: $color-primary;
            margin-bottom: 10px;
        }
        span{
            font-family: "Poppins", sans-serif;
            font-size: 9px;
            color: #958e9b;
            margin-top: 5px;
        }
        button{
            color: $color-primary;
        }
    }
}

// UTILITY
.presentation-img{
    min-height: 70%;
}
.col-30{
    width: 33%;
    flex-direction: column;
}
</style>