
<script>
export default {
    // definisco la props della lista
    props: {
        menuItems: {
            type: Array,
            required: true
        },
    }
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
                            <li v-for="item in menuItems" :key="item.text">
                                <a :href="item.href">{{item.text}}</a>
                            </li>
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
                            <h1>Buy Ans Sell Your <br> Car At Its Value</h1>
                            <p>Find the right price and dealer</p>
                            <button type="button" class="buttons btn-dark">Learn More<i class="fas fa-arrow-right" ></i></button>
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
            color: #fff;
            height: 700px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            h1 {
                font-size: 40px;
                font-weight: bold;
            }
            p{
                font-size: 15px;
                font-weight: bold;
            }
            .buttons{
                padding: 10px 0;
                max-width: 200px;
                display: flex;
                align-items: center; 
                padding: 12px 25px;
                color: #fff;
                background-color: rgb(29, 29, 29);
                border: none;
                font-size: 12px;
                font-weight: bold;
                cursor: pointer;
                text-align: center;
                gap: 8px; 
                i {
                    font-size: 16px; // Dimensione dell'icona
                }
            }
        }
    }

}
</style>