<script>
export default{
    name: 'SocialFooter'
}
</script>

<template>
    <section class="container-big d-flex">
            <div class="col-60">
                <p>
                    © Copyright 2012 - 2020 | Avada theme by ThemeFusion | All Rights Reseved | Powered by WordPress
                </p>
            
            </div>
            <div class="col-40">
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-pinterest-p"></i>

            </div>
        </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;
p{
    font-family: "Poppins", sans-serif;
    font-size: 9px;
    color: #958e9b;
    margin-bottom: 16px;
}
i{
    color: $color-primary;
    margin-left: 35px;
    font-size: 14px;
}


// UTILITY
.col-60{
    width: 60%;
}
.col-40{
    width: 40%;
    text-align: end;
}
</style>