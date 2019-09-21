<template>
    <section class="forgot__password container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-3"></div>
                <div class="col-md-6">
                    <div class="wrapper">
                    <div class="heading text-center">
                         <h3><router-link to="/" class="logo">farmcart.ng</router-link></h3>
                            <h4>Welcome Back</h4>
                            <p>Reset your password here</p>
                    </div>
                    <form>
                        <div class="form-group">
                            <div class="email-field d-flex justify-content-between">
                            <img src="../assets/pointer.svg" class="img-fluid email-icon" alt="">
                            <input type="email" class="form-control" placeholder="Enter email address *">
                            </div>
                        </div>
                        <button type="submit" class="password__btn">Reset Password</button>
                         <div class="bottom__text text-center mt-3">
                                <p>Don't have an account? <router-link to="/register" class="bottom-link">Register here</router-link></p>
                                <p>Already have an account? <router-link to="/login" class="bottom-link">Login</router-link></p>
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
    name:'ResetPassword'
}
</script>
<style lang="scss" scoped>
.wrapper{
      padding-top: 6rem;
      background:#fff;
    padding: 3rem;
    border-radius: 4PX;
}
.forgot__password{
    background: #EBECF1;
    height: 100vh;
    padding-top: 6rem;
}
.heading{
    font-family: 'Lato';
    color:#627081;
    padding-bottom: 1.2rem;
   .logo{
    text-decoration: none;
    color:rgb(68, 148, 46);
    font-weight: bold;
    font-family: 'Lato';
    font-size: 1.4rem;
    }
    h4{
        font-size: 1rem;
    }
    p{
        font-size: .9rem;
        // font-weight: bold;
    }
}
form{
    .email-field{
        border-bottom: 1px solid #ccc;
        .email-icon{
        height: 2rem;
        padding-top: .6rem;
    }
    input[type=email]{
        border:none;
        font-family: 'Lato';
        box-shadow: none;
         padding: 1.3rem 1rem;
        font-size: .9rem;
        color:#627081;
        background: transparent;
    }
    }
    .password__btn{
        background: rgb(68, 148, 46);
        width: 100%;
        color:#fff;
        padding: .6rem 0;
        font-family: 'Lato';
        border: none;
        font-size: .9rem;
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
</style>