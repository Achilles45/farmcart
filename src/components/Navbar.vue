<template>
    <div class="navbar__wrapper container-fluid">
        <div class="container">
            <div class="navbar__contents d-flex justify-content-between">
                <div class="logo"><h3><router-link to="/" class="logo">farmcart.ng</router-link></h3></div>
                <ul class="navbar__links d-flex justify-content-between">
                    <li><router-link to="/farmer" class="nav__link">Farmers</router-link></li>
                    <li><router-link to="/farm-shop" class="nav__link">Farm Shop</router-link></li>
                    <li><router-link to="/farm-shop" class="nav__link">Investor</router-link></li>
                    <li><router-link to="/register" class="nav__link">Register</router-link></li>
                    <li><router-link to="/contact" class="nav__link">Contact</router-link></li>
                    <li><router-link to="/login" class="nav__link">Login</router-link></li>
                </ul>
                <div @click="toggleNav()" class="navbar__toggler">
                    <i class="fa fa-bars"></i>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Navbar',
    methods:{
        toggleNav:function(){
            const nav = document.querySelector('.navbar__links');
            nav.classList.toggle('show-nav')
        }
    }
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.navbar__wrapper{
    // background: green;
    box-shadow: 0px 0px 3px rgba(0,0,0,.15);
    padding: .9rem 0;
    align-content: center !important;
    .logo{
        text-decoration: none;
        color:$primary-color;
        font-weight: bold;
        font-family: 'Roboto';
        font-size: 1.3rem;
    }
    .navbar__toggler{
        padding-top: .4rem;
        display: none;
        color:$primary-color;
        font-size: 1.5rem;
        font-weight: bold;
    }
    .navbar__links{
            margin: 0 !important;
            align-items: center;
        .nav__link{
           color:$primary-color;
           text-decoration:none;
           font-family: 'Lato', sans-serif;
           font-size:.8rem;
           padding-left: 1rem;
           font-weight: bold;
           opacity: .8;
           text-transform: uppercase;
        }
    }
}

//MEDIA QUERIES
@media only screen and (max-width: 768px){
    .navbar__links{
        flex-direction: column;
        background: $primary-color;
        position: absolute;
        padding: 5rem 3rem;
        top:4.354rem;
        z-index: 100;
        width: 100%;
        left: 0 !important;
        height: calc(100vh - 20%);
        display: none !important;
        line-height: 4;
        .nav__link{
            color:#fff !important;
            padding-left: 0 !important;
            font-size: .9rem !important;
        }
    }
    .navbar__toggler{
        display: block !important;
    }
    .show-nav{
        display: block !important;
        transition: all ease-in .5s;
    }
}
</style>