<script>
import SocialFooter from './SocialFooter.vue';

export default{
    name: 'AppFooter',
    props: ['navList'],
    components: {
        SocialFooter
    }
}
</script>

<template>
    <footer>
        <section class="container-big d-flex">
            <div class="col-60">
                <div class="container">
                    <!-- logo -->
                    <img src="../assets/images/avada-bakery-logo.png" alt="">
                    <!-- /logo -->
                    <!-- menu nav-bar -->
                    <nav>
                        <ul class="d-flex">
                            <li v-for="item in navList">{{ item.title }}</li>
                            <li>ORDES</li>
                            <li><i class="fa-solid fa-cart-shopping"></i></li>
                        </ul>
                    </nav>
                    <!-- /menu nav-bar -->
                </div>
            
            </div>
            <div class="col-40">
                <h5>Subscribe to our Newsletter</h5>
                <div class="subscribe d-flex">
                    <input type="email" placeholder="Enter email address*">
                    <button class="btn">Subscribe</button>
                </div>
            </div>
        </section>

        <SocialFooter></SocialFooter>

    </footer>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as*;
footer{
    height: 200px;
}

.container-big{
    align-items: start;
    justify-content: space-between;

    img{
        height: 45px;
    }

    ul{
        font-family: "Poppins", sans-serif;
        margin-top: 20px;

        li{
            color: $color-primary;
            margin: 0 10px;
            font-size: 12px;
            border-bottom: 1px solid transparent;

            &:hover{
                border-bottom: 1px solid $color-primary;
            }

            i{
                font-size: 12px;
            }
        }
    }
    h5{
        color: $color-primary;
        font-size: 18px;
    }
    .subscribe{
        justify-content: end;
        margin-top: 30px;

        input{
            width: 300px;
            border: 1px solid lightgray;
            border-radius: 6px;
            margin-right: 12px;
            padding: 9px 10px;
        }
        button{
            background-color: $bg-primary;
            color: white;
            
        }

    }
    
}

// UTILITY
.col-60{
    width: 60%;
}
.col-40{
    width: 40%;
    text-align: end;
}

.debug{
    border: 1px dashed black;
}
</style>