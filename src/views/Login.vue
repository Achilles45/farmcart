<template>
    <section class="login container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-3"></div>
                <div class="col-md-6">
                    <div class="login__form__wrapper">
                        <div class="heading text-center">
                            <h3><router-link to="/" class="logo">farmcart.ng</router-link></h3>
                            <h4>Welcome Back</h4>
                            <p>Please login to continue</p>
                        </div>
                        <form class="login__form">
                            <div class="form-group">
                                <div class="email__field d-flex justify-content-between">
                                    <img src="../assets/user.svg" class="img-fluid user__icon" alt="">
                                    <input type="text" class="form-control" placeholder="Email Address *">
                                </div>
                                </div>
                                <div class="form-group">
                                <div class="psssword__field d-flex justify-content-between">
                                    <img src="../assets/lock.svg" class="img-fluid password__icon" alt="">
                                    <input type="password" class="form-control" placeholder="Password *">
                                </div>
                            </div>
                            <button class="login__btn d-block" type="submit">Login</button>
                            <div class="bottom__text text-center mt-3">
                                <p>Don't have an account? <router-link to="/register" class="bottom-link">Register here</router-link></p>
                                <p>Forgot Password? <router-link to="/reset-password" class="bottom-link">Recover Password</router-link></p>
                            </div>
                        </form>
                    </div>
                </div>
                <div class="col-md-3"></div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'Login'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.login{
    background: #EBECF1;
    height: 100vh;
    // display: flex;
    // justify-content: center;
    // align-items: center;
    padding-top: 6rem;
    .login__form__wrapper{
        background:#fff;
        padding: 3rem;
        border-radius: 4PX;
        .logo{
        text-decoration: none;
        color:rgb(68, 148, 46);
        font-weight: bold;
        font-family: 'Lato';
        font-size: 1.4rem;
        }
        .heading{
            font-family: 'Lato';
            color:#627081;
            padding-bottom: 1.2rem;
            h4{
                font-size: 1rem;
            }
            p{
                font-size: .9rem;
                // font-weight: bold;
            }
        }
    }
    .login__form{
        .user__icon, .password__icon{
            height: 1.5rem;
            padding-top: .6rem;
        }
        .psssword__field, .email__field{
            border-bottom: 1px solid #ccc;
        }
        input[type=text], input[type=password]{
            border:none;
            box-shadow: none;
            padding: 1rem 1rem;
            font-size: .9rem;
            font-family: 'Lato';
            color:#627081;
            background: transparent;
            &::placeholder{
                color:#627081;
            }
        }
        .login__btn{
            background: rgb(68, 148, 46);
            width: 100%;
            color:#fff;
            padding: .6rem 0;
            font-family: 'Lato';
            border: none;
        }
        .bottom__text{
            font-family: 'Lato';
            p{
                font-size: .92rem;
                color:#627081;
                line-height: 1 !important;
            }
            .bottom-link{
                color:rgb(68, 148, 46);
                font-size: .9rem;
                // font-weight: bold;
            }
        }
    }
}
</style>