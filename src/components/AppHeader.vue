
<script>
export default {
    
}
</script>

<template lang="">
    <header>
        <div class="container">
            <div class="row gx-0">
                <div class="col-12 col-lg-6">
                    <div class="content-header">
                        <img src="../assets/logo-autocar11.png" alt="Logo" class="logo"/>
                        <ul class="nav-list list-unstyled">
                            <li><a href="#">Home</a></li>
                            <li><a href="#">About Us</a></li>
                            <li><a href="#">Vehicles</a></li>
                            <li><a href="#">Dealers</a></li>
                            <li><a href="#">Packages</a></li>
                            <li><a href="#">Blog</a></li>
                            <li><a href="#">Contact</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-12 col-lg-6">
                    <div class="content-header d-flex justify-content-center">
                        <button class="button-img">
                            <img class="item" src="../assets/padlock.png"/>
                            <span>My Account</span>
                        </button>
                        <button class="button-img">
                            <img class="item" src="../assets/add.png"/>
                            <span>Add Car</span>
                        </button>
                        <div class="icon">
                            <i class="fa-solid fa-bars"></i>
                        </div>
                        <button class="button-img">
                            <img class="item" src="../assets/headphones.png"/>
                            <span>+1(234) 567 89 10</span>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </header>
    <div class="jumbotron">
        <div class="sfondo">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <div class="content-jumbo">
                            <!-- contenuto + immagine di sfondo -->
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>

header {
    background-color: #fff;
}

.container {
    .content-header {
        display: flex;
        align-items: center;
        padding: 10px 0;
        
        .logo {
            width: 150px;
            height: auto;
            margin-right: 20px; 
        }

        .nav-list {
            display: flex;
            gap: 12px; 
            align-items: center;
            flex-wrap: nowrap; 
            overflow-x: auto; 
            margin-bottom: 0;

            li {
                white-space: nowrap; 
            }

            a {
                text-decoration: none;
                color: black;
                font-size: 15px;
                font-weight: 500;
            }
        }
        .button-img {
            background-color: #000;
            padding: 10px;
            color: #fff;
            border: none;
            border-radius: 5px;
            margin: 0 5px;
            white-space: nowrap;
            max-width: 150px;
            overflow: hidden;
            
            .item {
                filter: invert(1);
                width: 25px;
                height: auto;
            }

            span {
                font-size: 12px;
                font-weight: bold;
            }
        }
        .icon{
            font-size: 25px;
            margin: 0 5px;
        }
    }

}

.jumbotron{
    background-color: #000;
    padding: 10px 0;
    .sfondo{
        background-image: url('../assets/slider-autocar-5.jpg');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        .content-jumbo{
            height: 700px;
            border: 1px dashed white ;
        }
    }

}
</style>