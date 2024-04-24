<script>
export default{
    name: 'AppDelivery'
}
</script>

<template>
    <section class="delivery">
        <div class="container-small d-flex">
            <!-- testo informativo -->
            <div class="text-info">
                <span>TRY OUR SEASONAL PRODUCTS</span>
                <h4>
                   Order for pick-up or delivery to your home
                </h4>
                <button class="btn">Shop Now</button>
            </div>
            <!-- /testo informativo -->
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;
.delivery{
    background-image: url(../assets/images/call-to-action-bg.jpg);
    background-size: cover;
    height: 300px;
    margin-bottom: 20px;
    

    .container-small{
        height: 100%;
        align-items: center;

        .text-info{
            width: 60%;
    
            span{
                font-size: 10px;
                font-family: "Poppins", sans-serif;
                color: #958e9b;
            }
            h4{
                color: white;
                font-weight: 800;
                font-size: 30px;
                margin: 10px 0;
            }
            button{
                margin-top: 30px;
            }
        }
    }
}
</style>