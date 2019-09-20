<template>
    <section class="farms">
        <div class="container">
            <div class="row">
                <div class="col-12 heading text-center">
                    <h3>Our Farms</h3>
                </div>
            </div>
            <div class="farms__wrapper">
               <div class="farm__card" v-for="(farm, index) in Farms" :key="index">
                   <img :src="farm.image" class="img-fluid" alt="">
                   <div class="card__body">
                        <h5>{{ farm.name}}</h5>
                        <h6>{{ farm.location }}</h6>
                        <div class="farm__details d-flex justify-content-between">
                            <div class="farm__details_-left">
                                <small>Duration</small>
                                <p>{{ farm.duration }}</p>
                                <small>Price</small>
                                <p>&#8358;{{ farm.price }}</p>
                            </div>
                            <div class="farm__details__right">
                                <small>Returns</small>
                                <h2>{{ farm.returns }}</h2>
                            </div>
                        </div>
                        <!-- <div class="button__wrapper text-center">
                            <button class="farm__btn">Fund</button>
                        </div> -->
                    </div>
               </div>
                </div>
                 <div class="farm__button text-center pb-5 pt-3">
                   <router-link to="farm-shop" class="farm-btn">See more &nbsp;&nbsp;<i class="fa fa-long-arrow-right"></i></router-link>
               </div>
            </div>
    </section>
</template>
<script>
export default {
    name: 'Farm',
    data(){
        return{
            Farms:[
                {
                    id:1,
                    image:require('../assets/maize.jpg'),
                    name: 'Maize Farm',
                    price: '35,000',
                    location:'Kaduna State',
                    duration: '9 months',
                    returns:'25%'
                },
                 {
                    id:2,
                    image:require('../assets/fish.jpeg'),
                    name: 'Fish Farm',
                    price:'50,000',
                    location:'Delta State',
                    duration: '6 months',
                    returns:'40%'
                },
                {
                    id:3,
                    image:require('../assets/soyabeans.jpeg'),
                    name:'Soyabeans Farm',
                    price:'40,000',
                    location:'Kano State',
                    duration: '5 months',
                    returns:'30%'
                },
                {
                    id:4,
                    image:require('../assets/pig.jpeg'),
                    name:'Pig Farm',
                    price:'70,000',
                    location:'Ondo State',
                    duration: '15 months',
                    returns:'45%'
                }
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.farms{
    background: $primary-color;
    margin-top: 1rem;
    color:#fff;
    .heading{
        padding: 3rem 0;
        h3{
            font-family: 'Roboto';
            font-size: 1.3rem;
            text-shadow: 0.03em 0.03em 0.05em #fff;
            text-transform: uppercase;
        }
    }
        .farm-btn{
            background: rgb(68, 148, 46);
            padding: .8rem 3rem;
            text-decoration: none;
            color:#fff;
            font-family: 'Lato';
            font-size: .9rem;
            font-weight: bold;
            border-radius: 3px;
        }
    .farms__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        grid-gap: 20px;
        padding-bottom: 2rem;
        .farm__card{
            background: #fff;
            border-top-left-radius: 4px;
            border-top-right-radius: 4px;
            cursor: pointer;
            .card__body{
                padding: 1rem 1.5rem;
                font-family: 'Lato';
                box-shadow: 4px 0px 40px 0px rgba(0,0,0,.5);
                h5{
                    color:$primary-color;
                    font-weight: bold;
                    font-size: 1.1rem;
                }
                h6{
                    color:#627081;
                }
                h2{
                      color:$primary-color;
                }
                small{
                    color:#484848;
                    font-weight: normal;
                }
                p{
                    color:#333;
                }
                .farm__btn{
                    background: $primary-color;
                    border:none;
                    padding: .5rem 1.5rem;
                    border-radius: 20px;
                    color:#fff;
                    font-size: .75rem;
                    font-weight: bold;
                }
            }
            .farm-img{
                width: 100%;
                height: auto;
                border-top-left-radius: 4px;
                border-top-right-radius: 4px;
            }
        }
    }
}
</style>