<template>
    <section class="process">
        <div class="container-fluid">
            <div class="container">
                <div class="row">
                    <div class="col-12 heading text-center">
                        <h4>How it Works</h4>
                        <p>Our process and approach is very simple and convinient for anyone</p>
                    </div>
                </div>
                <div class="process__wrapper">
                        <div class="process__card">
                            <img src="../assets/farmer-icon.png" class="process__img" alt="">
                            <h5>Browse our Farms</h5>
                            <p>We work with small scale farmers with the potential to scale. You can browse through our farm shop and select the one you want to sponsor.</p>
                        </div>
                         <div class="process__card">
                            <img src="../assets/invest-icon.png" class="process__img" alt="">
                            <h5>Make payment</h5>
                            <p>You then proceed to make your investment on the farm of your choice. Payments can be made through direct bank transfer, paystack or card payment.</p>
                        </div>
                         <div class="process__card">
                            <img src="../assets/chart.png" class="process__img" alt="">
                            <h5>Get Returns</h5>
                            <p>See how your farm is performing from any device. We also send wekkly report on your farm performance. Cash out at the stipulated time from your dashboard.</p>
                        </div>
                    </div>
                </div>
            </div>
    </section>
</template>
<script>
export default {
    name: 'Process'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.process{
    margin-top: 3rem;
    .heading{
        font-family: 'Lato';
        h4{
            color:$primary-color;
        }
        p{
            color:#627081;
        }
    }
    .process__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 20px;
        margin: 2rem 0;
        .process__card{
            box-shadow: 0px 0px 3px rgba(0,0,0,.15);
            border-radius: 3px;
            padding:2rem;
            .process__img{
                max-width: 80px;
                height: auto;
                padding: 1rem 0;
            }
            h5{
                font-family: 'Roboto';
                color:$primary-color;
                font-size: 1.1rem;
                padding-bottom: .3rem;
            }
            p{
                font-family: 'Lato';
                color:#627081;
                font-size: .9rem;
            }
        }
    }
}

//Media queries
@media only screen and (max-width: 768px){
    //   .process__card{
    //       margin-right: 1rem !important;
    //   }
}
</style>