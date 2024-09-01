<script>
export default {
    
}
</script>


<template lang="">
    <footer>
        <div class="container">
            <div class="row gy-3">
                <div class="col-12 col-md-6 col-lg-2">
                    <div class="content-footer">
                        <div class="footer-logo">
                            <img class="img-fluid" src="../assets/logo-footer-autocar11.png"/>
                        </div>
                        <div class="footer-icons">
                            <div class="icon">
                                <i class="fa-solid fa-location-dot"></i>
                                <span>New Jersey, USA</span>
                            </div>
                            <div class="icon">
                                <i class="fa-solid fa-phone"></i>
                                <span>+1 (234) 567 89 10</span>
                            </div>
                            <div class="icon">
                                <i class="fa-regular fa-envelope"></i>
                                <span><a>example@example.com</a></span>
                            </div>
                        </div>
                        <div class="social">
                            <i class="fa-brands fa-facebook-f"></i>
                            <i class="fa-brands fa-instagram"></i>
                            <i class="fa-brands fa-twitter"></i>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-6">
                    <div class="content-footer">
                        <h4>Join Our Newsletter</h4>
                        <p>Subscribe to be informed about our services and products.</p>
                        <div class="form">
                            <input type="text" placeholder="Your Email Address"/>
                            <div>
                                <button>Subscribe</button>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-2">
                    <div class="content-footer">
                        <h4>My Account</h4>
                        <ul class="list-unstyled footer-list">
                            <li class="footer-list-item"><i class="fas fa-minus"></i>My Account</li>
                            <li class="footer-list-item"><i class="fas fa-minus"></i>Checkout</li>
                            <li class="footer-list-item"><i class="fas fa-minus"></i>Cart</li>
                            <li class="footer-list-item"><i class="fas fa-minus"></i>Packages</li>
                            <li class="footer-list-item"><i class="fas fa-minus"></i>Add Car</li>   
                        </ul>
                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-2">
                    <div class="content-footer">
                        <h4>My Account</h4>
                        <ul class="list-unstyled footer-list">
                            <li class="footer-list-item"><i class="fas fa-minus"></i>Home</li>
                            <li class="footer-list-item"><i class="fas fa-minus"></i>About Us</li>
                            <li class="footer-list-item"><i class="fas fa-minus"></i>Blog</li>
                            <li class="footer-list-item"><i class="fas fa-minus"></i>Contact</li>
                            <li class="footer-list-item"><i class="fas fa-minus"></i>Refind &amp; Returns</li>   
                        </ul>
                    </div>
                </div>
                <div class="col-12">
                    <div class="content-footer-bottom d-flex justify-content-center align-items-center ">
                        <p>2022 Autocar - All Rights Reserved</p>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer{
    padding: 30px 0;
    background-color: black;
    .container{
        .content-footer{
            border: 1px solid white;
            color: white;
        }
        .content-footer-bottom{
            height: 100px;
            border: 1px solid white;
            p{
                color: white;
                font-size: 14px;
            }
        }
    }
}

</style>