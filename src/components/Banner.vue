<template>
    <section class="banner__section">
        <div class="banner__contents container-fluid">
            <div class="container">
                <div class="row">
                    <div class="col-md-6 col-sm-12 col-xs-12">
                        <h1>Farming in the cloud</h1>
                        <p>We enable you to participate in the agricultural value chain virtually by empowring local farmers while making competitive returns on invetsments</p>
                        <router-link to="/register" class="hero__btn">Get Started</router-link>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'Banner'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.banner__section{
    background: url('../assets/farmer5.jpg');
    box-shadow: inset 0 0 0 1000px rgba(0,0,0,.65);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    padding: 10rem 0;
    position: relative;
    z-index: -100;
    .banner__contents{
        color:#fff;
        h1{
            font-weight: 800;
            text-shadow: 0.01em 0.01em 0.05em #fff;
            font-size: 2.5rem;
            font-family: 'Roboto';
            text-transform: uppercase;
            letter-spacing:1px;
        }
        p{
            font-family: 'Roboto';
            padding: .8rem 0;
            opacity: .8;
            letter-spacing: .2px;
            word-spacing: .5px;
            font-size: .9rem;
            line-height: 1.5;
        }
        .hero__btn{
            background: $primary-color !important;
            color: #fff;
            text-decoration: none;
            padding: .9rem 4rem;
            border-radius: 2px;
            font-family: 'Roboto';
            font-size: .9rem;
        }
    }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px) {
       .banner__contents{
           h1{
               text-shadow: none !important;
               font-size: 1.5rem !important;
               font-weight: normal;
           }
           p{
               opacity: .9 !important;
               font-size: 1rem;
           }
       }
}
</style>