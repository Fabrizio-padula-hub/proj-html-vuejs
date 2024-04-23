<script>
export default{
    name: 'AppSpecialMoments'
}
</script>

<template>
    <section class="container-big">
        <div class="title">
            <span>CORPORATE & WEDDINGS</span>
            <h3>Baking Special Moments</h3>
        </div>
        <div class="pictures d-flex g-50">
            <div>
                <img src="../assets/images/corporate-bg.jpg" alt="">
            </div>
            <div>
                <img src="../assets/images/wedding-bg.jpg" alt="">
            </div>
        </div>
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
.pictures{
    img{
        object-fit: cover;
        margin: 20px 0;
    }
    
}
</style>