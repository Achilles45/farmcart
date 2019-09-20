<template>
    <footer>
        <hr />
        <div class="footer__contents container-fluid">
            <div class="container">
                <div class="row">
                    <div class="col-md-8">
                        <h4>About Farmcart</h4>
                        <p>Farmcart is an agricultural crowdfunding paltform that seeks to connect small holder farmers to capital while providing competitive returns for investors. The company seeks to provide value in the entire agricultural value chain for both farmers and investors with a view on ending hunger</p>
                        <p> <small>Contact Detials:</small> 1 Adani Road, Off NYSC Camp, Enugu, Enugu State</p>
                        <small>support@farmcart.com 08103515205 Mondays to Fridays: 9am to 5pm</small>
                    </div>
                    <div class="col-md-4">
                        <div class="row">
                            <div class="col-md-6">
                                <h5>Quick Links</h5>
                                <ul>
                                    <li><router-link to="/register" class="footer-links">Register</router-link></li>
                                    <li><router-link to="/login" class="footer-links">Login</router-link></li>
                                    <li><router-link to="/carriers" class="footer-links">Careers</router-link></li>
                                    <li><router-link to="/Policy" class="footer-links">Policy</router-link></li>
                                    <li><router-link to="/terms" class="footer-links">Terms & Condition</router-link></li>
                                </ul>
                            </div>
                            <div class="col-md-6">
                                <h5>Get Social</h5>
                                <a href="#"><i class="fa fa-facebook-f"></i></a>
                                <a href="#"><i class="fa fa-twitter"></i></a>
                                <a href="#"><i class="fa fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="footer-bottom pt-2">
                    <small>Copyright &copy; 2019. All rights reserved. Farmcart Limited</small>
                </div>
            </div>
        </div>
    </footer>
</template>
<script>
export default {
    name: 'Footer'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
footer{
    .footer__contents{
        padding: 4rem 0; 
       h4{
           font-family: 'Lato';
       }
       p{
           font-family: 'Lato';
           font-size: .9rem;
           color:#627081;
       }
       small{
           color:#627081;
           font-size: .9rem;
       }
       hr{
           background:red !important;
       }
       h5{
           font-family: 'Lato';
       }
       .footer-links{
            color:#627081;
            text-decoration: none;
       }
       .fa-facebook-f, .fa-twitter, .fa-instagram{
           padding-right: .5rem;
           font-size: 1.2rem;
       }
    }
}
</style>