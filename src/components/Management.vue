<template>
    <section class="management container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-5 pt-3">
                    <h2>Intuitive management tool!</h2>
                    <p>We have provided an intuitive dashboard for farmers and investors to be able to manage their farms in real time and get a sense of performance. You can get access to more investment opportunities we bring your way on the deashboard.</p>
                    <div class="button mb-5">
                        <router-link to="/register" class="management__btn">Become an Investor</router-link>
                    </div>
                </div>
                <div class="col-md-1"></div>
                <div class="col-md-6 pb-5">
                    <img src="../assets/dashboard.png" class="img-fluid dashboard" alt="">
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name:'Management'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.management{
    margin: 4rem 0;
    h2{
        font-family: 'Lato';
        text-transform: capitalize;
        color:#3c3c3c;
        // font-weight: bold;
    }
    p{
        font-family: 'Lato';
        color: #627081;
        padding-top: 1rem;
        padding-bottom: 2rem;
    }
    .management__btn{
        background: $primary-color;
        color:#fff;
        padding:.95rem 2rem;
        text-decoration: none;
        border-radius: 2px;
        font-family: 'Lato';
        font-size: .95rem;
        &:hover{
            background: #48AF2C;
            transition: all ease-in-out .5s;
        }
    }
    .dashboard{
        animation-name: animate;
        animation-duration: 4.5s;
        animation-iteration-count: infinite;
        animation-direction: alternate;
    }
}

//Animation
@keyframes animate{
    from{
        transform: translateY(-30px);
    }
    to{
          transform: translateY(30px);
    }
}
</style>