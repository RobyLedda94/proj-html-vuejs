

<script>
export default {
    props : {
        filters: {
            type: Array,
        },
        vehicles: {
            type: Array,
        },
        cards: {
            type: Array,
        },
        testimonials: {
            type: Array,
        },
        carsBottom: {
            type: Array,
        },
    }
}
</script>

<template lang="">
    <main>
        <!-- sezione top main -->
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="content-main-top-li px-3">
                        <ul class="list-unstyled d-flex justify-content-between align-items-center mb-0">
                            <li v-for="filter in filters" :key="filter">{{ filter.text}}
                                <i :class="filter.icon"></i>
                            </li>
                          </ul>
                    </div>
                </div>
            </div>
            <div class="row g-0 my-3">
                <div class="col-12 col-md-4 col-lg-2" v-for="vehicle in vehicles" :key="vehicle">
                    <div class="content-main-top-type">
                        <img class="img-fluid" :src="vehicle.image"/>
                        <div class="text-content">
                            <p class="title mb-0">{{ vehicle.title }}</p>
                            <p class="listings mb-2">{{ vehicle.listings }} Listings</p>
                        </div>
                    </div>
                </div>
            </div>
            <!-- parte main center carte auto -->
            <div class="row g-0 mb-5">
                <div class="col-12 col-md-6 col-lg-3" v-for="card in cards" :key="card">
                    <div class="content-main-center-card">
                        <img class='card-img-top' :src="card.image"/>
                        <div class="card-body">
                            <div class='card-description'>
                                <p class='model'>{{ card.model }}<i class="fas fa-check"></i></p>
                                <p>{{ card.type }}</p>   
                            </div>
                            <div class="card-details d-flex">
                                <div class='price'>
                                    <i class="fas fa-dollar-sign"></i> {{ card.price }}
                                </div>
                                <div class='brand'>
                                    <i class="fas fa-car"></i> {{ card.brand }}
                                </div>
                                <div class='fuel'>
                                    <i class="fas fa-gas-pump"></i> {{ card.fuel }}
                                </div>
                                <div class='heart'>
                                    <i class="fas fa-heart"></i>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-12 mt-3">
                    <div class="content-main text-center">
                        <button type="button" class="buttons btn-dark">Show All Cars<i class="fas fa-arrow-right" ></i></button>
                    </div>
                </div>
            </div>
        </div>
        <!-- sezione about -->
        <div class="container-sm">
            <div class="row">
                <div class="col-12 col-lg-8">
                    <div class="content-main-sm">
                        <div class="image-container">
                            <img class="img-fluid img-0" src="../assets/circle-auto-car-1.png" alt="immagine 0"/>
                            <img class="img-fluid img-1" src="../assets/aoutcar-about-1.png" alt="immagine 0"/>
                            <div class="circle circle-top">
                                <p class="mb-0 fs-4">24</p>
                                <p>Years of <br> Experience</p>
                            </div>
                            <div class="circle circle-bottom">
                                <p class="mb-0 fs-4">240</p>
                                <p>Special Expert<br>Team</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-lg-4">
                    <div class="content-main-sm py-5">
                        <div class="top-right">
                            <h4>Want to buy or sell a vehicle?</h4>
                            <p class="text">You can put your vehicles for sale by by registering on out website. Whether you are a dealer or sell personally. Sell your vehicle in the most portable way. With this system, which has millions of members, you vill be able to buy and sell vehicles quikly.</p>
                        </div>
                        <div class="bottom-right mt-5">
                            <div class="models">
                                <i class="fa-solid fa-car"></i>
                                <div class="text-box">
                                    <h6>Model Vehicles</h6>
                                    <p class="text">We are sure that you will find vehicles of suitable models on our website</p>
                                </div>
                            </div>
                            <div class="models">
                                <i class="fa-solid fa-car-burst"></i>
                                <div class="text-box">
                                    <h6>2nd Hand Vehicles</h6>
                                    <p class="text">We are sure that you will find vehicles of suitable models on our website</p>
                                </div>
                            </div>
                            <button type="button" class="buttons btn-dark">Get to know us<i class="fas fa-arrow-right" ></i></button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- sezione testimonials -->
        <div class="jumbotron mb-5">
            <div class="container my-3">
                <div class="row gy-3">
                    <div class="col-12">
                        <div class="content-main-jumbo text-center">
                            <div class="jumbo-icons">
                                <div class="like">
                                    <i class="fa-regular fa-thumbs-up fa-3x"></i>
                                </div>
                                <div class="stars">
                                    <i class="fa-regular fa-star"></i>
                                    <i class="fa-regular fa-star"></i>
                                    <i class="fa-regular fa-star"></i>
                                </div>
                            </div>
                            <h3>What Are Our Custumers Sayng ?</h3>
                            <p>Opinion from our happy costumers</p>
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-3" v-for="testimonial in testimonials" :key="testimonial">
                        <div class="content-main-testimonial-card">
                            <div class="testimonial-text">
                                <p>{{testimonial.text}}</p>
                            </div>
                            <div class="testimonial-img">
                                <img :src="testimonial.image"/>
                            </div>
                            <div class="testimonial-name">
                                <p>{{testimonial.name}}</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-12">
                        <div class="content-main-jumbo mb-3">
    
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="container mb-5 py-5">
            <div class="row gy-2">
                <div class="col-12">
                    <div class="content-main-bottom py-2">
                        <div class="circle">
                            <i class="fa-regular fa-thumbs-up fa-3x"></i>
                        </div>
                        <div class="text text-center">
                            <h4>Resent Articles</h4>
                            <p>Useful information about car.</p>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-3" v-for="car in carsBottom" :key="car">
                    <div class="content-main-bottom-cards">
                        <img class="img-fluid" :src="car.image"/>
                        <div class="card-body">
                            <p>{{ car.date}} </p>
                            <h5 class="card-title">{{car.title}}</h5>
                            <p class="card-text">{{car.text}}</p>
                            <button class="buttons btn-dark">More</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
    </main>
</template>

<style lang="scss" scoped>
.content-main-top-li{
    padding: 25px 0;
    .list-unstyled{
        display: flex;
        flex-wrap: nowrap;
        justify-content: space-between;
        li {
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative; 
            font-size: 12px;
            flex-basis: calc(100% / 8);
            max-width: calc(100% / 8);
            flex-grow: 0;
            padding: 15px;
            border: 1px solid #aaa;
            color: #aaa;
            border-radius: 5px;
            margin: 0 5px;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
            text-align: center; 
            i{
                position: absolute;
                right: 10px; 
            } 
            &:hover{
                background-color: black;
                color: #fff;
                font-weight: bold;
            }
        }
    }
}

.content-main-top-type{
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    border: 1px solid #aaa;
    overflow: hidden; 
    background-color: #fff;
    border: 1px solid #eee;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s;
    &:hover{
        transform: scale(1.05)
    }
    .listings{
        font-size: 12px;
    }
}

.content-main-center-card{
    border: 1px solid #ddd;
    overflow: hidden; 
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    background-color: #fff;
    padding: 10px;
    position: relative;
    transition: transform 0.3s, box-shadow 0.3s;
    &:hover {
        transform: scale(1.05);
        z-index: 1;
    }
    .card-body{
        font-size: 13px;
        .card-description{
            margin-top: 5px;
            i{
                background-color: black; 
                color: white;
                padding: 3px;
                border-radius: 50%;
                margin-left: 3px;
                font-size: 12px;
            }
        }
        .card-img-top{
            width: 100%;
            height: auto;
        }
        .card-details div{
            margin: 0 5px 0 0;
        }
        .heart{
            position: absolute;
            right: 0;
            color: #aaa;
        }
        .heart:hover{
            color: red;
        }
    }


}

.content-main{
    
    .buttons{
        padding: 12px 25px;
        color: #fff;
        background-color: black;
        border: none;
        font-size: 12px;
        font-weight: bold;
        &:hover {
            transform: scale(1.02);
        }
        i{
            margin-left: 5px;
        }
    }
}

.container-sm{
    padding: 0 70px;
    margin-bottom: 70px;
    
    .content-main-sm{
        .text{
            color: #777777;
            font-size: 14px;
        }
        .buttons{
            padding: 12px 25px;
            color: #fff;
            background-color: black;
            border: none;
            font-size: 12px;
            font-weight: bold;
            &:hover {
                transform: scale(1.02);
            }
            i{
                margin-left: 5px;
            }
        }
        .image-container{
            position: relative;
            .img-1{
                position: absolute;
                top: 0;
                left: 0;
            }
            .circle{
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                text-align: center;
                color: #fff;
                background: black;
                border-radius: 50%;
                font-weight: bold;
                max-width: 10%; 
                max-height: 10%;
                padding: 60px; 
            }
            .circle-top{
                position: absolute;
                top: 25%;
                left: 25%;
                
                transform: translate(-50%, -50%);
            }
            .circle-bottom{
                position: absolute;
                bottom: 25%;
                right: 25%;
                transform: translate(50%, 50%);
            }
        }
        .models{
            display: flex;
            align-items: center;
            gap: 10px;
            i{
                font-size: 30px;
                color: #414141;

            }
            .text-box{
                .text{
                    color: #777777;
                    font-size: 12px;
                }
            }
    
        }

    }

}

.jumbotron{
    padding:50px 0;
    background-image: url('../assets/comment-bg-autocar.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    .content-main-jumbo{
        color: #fff;
    }
    .jumbo-icons{
        display: flex;
        flex-direction: column;
        align-items: center;
        .stars{
            i{
                font-size: 15px;
            }
        }
    }
    .content-main-testimonial-card{
        background-color: #fff;
        border-radius: 10px;
        text-align: center;
        padding: 40px 30px;
        min-height: 405px;
        transition: transform 0.1s;
        &:hover{
            transform: scale(1.05)
        }
        .testimonial-text{
            font-size: 14px;
            color: #777777;
            margin-bottom: 35px;
        }
        .testimonial-img img{
            width: 90px;
            margin-bottom: 50px;
        }
        .testimonial-name{
            font-size: 15px;
            color: #777777;
        }
    }

}

.content-main-bottom{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    .circle{
        display: flex;
        background-color: black;
        padding: 10px;
        border-radius: 50%;
        margin-bottom: 5px;
        i{
            color: #fff;
        }
    }
    .text{
        h4{
            font-size: 24px;
            font-weight: bold;
        }
        p{
            font-size: 12px;
            color: #777777;
        }
    }
}

.content-main-bottom-cards{
    min-height: 385px;
    text-align: center;
    padding: 15px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    .card-title{
        font-weight: bold;
        margin-bottom: 20px;
    }
    .card-text {
        font-size: 13px;
        color: #777777;
    }
    .buttons{
        padding: 12px 25px;
        color: #fff;
        background-color: black;
        border: none;
        font-size: 12px;
        font-weight: bold;
        &:hover {
            transform: scale(1.02);
        }
    }
}


/*-------------------media-----------------*/

@media (max-width: 768px) {
    .content-main-top-li .list-unstyled {
        flex-wrap: wrap; 
    }
    .content-main-top-li .list-unstyled li {
        flex-basis: calc(50% - 10px);
        max-width: calc(50% - 10px);
        margin-bottom: 10px;
    }
}

@media (max-width: 576px) {
    .content-main-top-li .list-unstyled li {
        flex-basis: calc(100% - 10px); 
        max-width: calc(100% - 10px);
    }
}



</style>