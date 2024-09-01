<script>
export default {
    // definisco la props
    props: {
        footerLists: {
            type: Array,
        }
    }
    
}
</script>


<template lang="">
    <footer>
        <div class="container">
            <div class="row gy-3">
                <div class="col-12 col-md-6 col-lg-2">
                    <div class="content-footer">
                        <div class="footer-logo mb-4">
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
                    <div class="content-footer mx-3">
                        <h4>Join Our Newsletter</h4>
                        <p>Subscribe to be informed about our services and products.</p>
                        <div class="form">
                            <input type="text" placeholder="Your Email Address"/>
                            <button>Subscribe<i class="fas fa-arrow-right mx-2" ></i></button>
                        </div>
                    </div>
                </div>
                <!-- ciclo la colonna -->
                <div v-for="(list, index) in footerLists" :key="index" class="col-12 col-md-6 col-lg-2">
                    <div class="content-footer">
                        <h4>{{ list.title }}</h4>
                        <ul class="list-unstyled footer-list">
                            <li v-for="(item, i) in list.items" :key="i" class="footer-list-item"><i class="fas fa-minus"></i>{{ item }}</li>  
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
            color: white;
            font-size: 13px;
            .footer-icons{
                margin-bottom: 25px;
                .icon{
                    display: flex;
                    align-items: center;
                    margin-bottom: 15px;
                    i{
                        margin-right: 10px;
                        font-size: 20px;
                    }
                }
            }
            .social{
                display: flex;
                justify-content: center;
                gap: 30px;
                font-size: 20px;
                
            }
            h4{
                margin: 20px 0;
                font-weight: bold;
                
            }
            p{
                font-size: 12px;
            }
            .form{
                display: flex;
                flex-direction: column;
                align-items: start;
                justify-content: center;
                width: 100%;
                input{
                    width: 50%;
                    padding: 10px;
                    margin-bottom: 3px;
                }
                button{
                    width: 50%;
                    padding: 10px;
                    border: none;
                    cursor: pointer;
                    color:#777777;
                }
            }
            .footer-list{
                .footer-list-item{
                    margin-bottom: 15px;
                    font-size: 12px;
                    i{
                        margin-right: 10px;
                        font-size: 15px;
                        font-weight: bold;
                    }
                }
            }
        }
        .content-footer-bottom{
            height: 100px;
            p{
                color: white;
                font-size: 14px;
            }
        }
    }
}

</style>