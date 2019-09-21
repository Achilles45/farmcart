<template>
    <section class="register container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-3"></div>
                <div class="col-md-6">
                    <div class="register__contents">
                     <!-- <div class="heading text-center">
                            <h3><router-link to="/" class="logo">farmcart.ng</router-link></h3>
                            <h4>Start farming today</h4>
                            <p>Create a free account to begin!</p>
                        </div> -->
                        <form class="register__form">
                            <div class="row">
                                <div class="col-md-6">
                                    <div class="form-group">
                                        <div class="name__field d-flex justify-content-between">
                                            <img src="../assets/user.svg" class="img-fluid user-icon" alt="">
                                            <input type="text" class="form-control" placeholder="First Name *">
                                        </div>
                                    </div>
                                </div>
                                <div class="col-md-6">
                                    <div class="form-group">
                                        <div class="name__field d-flex justify-content-between">
                                            <img src="../assets/user.svg" class="img-fluid user-icon" alt="">
                                            <input type="text" class="form-control" placeholder="Last Name *">
                                        </div>
                                    </div>
                                </div>
                            </div><br />
                             <div class="row">
                                <div class="col-md-6">
                                    <div class="form-group">
                                        <div class="name__field d-flex justify-content-between">
                                            <img src="../assets/user.svg" class="img-fluid user-icon" alt="">
                                            <input type="text" class="form-control" placeholder="Username Name *">
                                        </div>
                                        <small class="text-muted">Please make sure your username is unique</small>
                                    </div>
                                </div>
                                <div class="col-md-6">
                                    <div class="form-group">
                                        <div class="name__field d-flex justify-content-between">
                                            <img src="../assets/pointer.svg" class="img-fluid user-icon" alt="">
                                            <input type="email" class="form-control" placeholder="Email address *">
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="form-group">
                            <div class="name__field d-flex justify-content-between">
                                <img src="../assets/pointer.svg" class="img-fluid user-icon" alt="">
                                <input type="tel" class="form-control" placeholder="Phone number *">
                            </div>
                            </div>
                            <div class="row">
                                <div class="col-md-6">
                                    <div class="form-group">
                                         <div class="name__field d-flex justify-content-between">
                                <img src="../assets/lock.svg" class="img-fluid user-icon" alt="">
                                <input type="tel" class="form-control" placeholder="Password *">
                            </div>
                                    </div>
                                </div>
                                <div class="col-md-6">
                                    <div class="form-group">
                                         <div class="name__field d-flex justify-content-between">
                                <img src="../assets/lock.svg" class="img-fluid user-icon" alt="">
                                <input type="tel" class="form-control" placeholder="Confirm Password *">
                            </div>
                                    </div>
                                </div>
                            </div>
                            <button type="submit" class="register__btn">Register</button>
                            <div class="bottom__text text-center mt-3">
                                <p>Don't have an account? <router-link to="/login" class="bottom-link">Login</router-link></p>
                                <small>By clicking register, you agree to our <router-link to="/" class="bottom-link">terms & conditions</router-link></small>
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
    name: 'Register'
}
</script>
<style lang="scss" scoped>
.register{
    background: #EBECF1;
    height: 100vh;
}
.register__contents{
    padding-top: 6rem;
.heading{
.logo{
    text-decoration: none;
    color:rgb(68, 148, 46);
    font-weight: bold;
    font-family: 'Lato';
    font-size: 1.4rem;
    }
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
.register__form{
    .user-icon{
        height: 1.5rem;
        padding-top: .6rem;
    }
    .name__field{
         border-bottom: 1px solid #ccc;
    }
    input[type=text], input[type=email], input[type=password], input[type=tel]{
        border:none;
        box-shadow: none;
        padding: 1rem 1rem;
        font-size: .9rem;
        font-family: 'Lato';
        color:#627081;
        background: transparent;
    }
    small{
        font-size: .8rem;
        color:#627081;
    }
    .register__btn{
        background: rgb(68, 148, 46);
        width: 100%;
        color:#fff;
        padding: .6rem 0;
        font-family: 'Lato';
        border: none;
    }
}
 .bottom__text{
            font-family: 'Lato';
            padding-top: 1rem;
            p{
                font-size: .92rem;
                color:#627081;
                line-height: .1 !important;
            }
            .bottom-link{
                color:rgb(68, 148, 46);
                font-size: .9rem;
                // font-weight: bold;
            }
        }
}
</style>