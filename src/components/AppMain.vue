

<script>
export default {
    
}
</script>

<template lang="">
    <main>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="content-main-top-li px-3">
                        <ul class="list-unstyled d-flex justify-content-between align-items-center mb-0">
                            <li>Keywords</li>
                            <li>Location</li>
                            <li>All Categories</li>
                            <li>Brand</li>
                            <li>Fuel Type</li>
                            <li>Trasmission</li>
                            <li>Status</li>
                            <li>Search</li>
                          </ul>
                    </div>
                </div>
            </div>
            <div class="row g-0">
                <div class="col-12 col-md-4 col-lg-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-12 col-md-4 col-lg-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-12 col-md-4 col-lg-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-12 col-md-4 col-lg-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-12 col-md-4 col-lg-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-12 col-md-4 col-lg-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
            </div>
            <div class="row g-0 mb-3">
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-top-cars"></div>
                </div>
            </div>
            <div class="row g-0 mb-5">
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-12 mt-2">
                    <div class="content-main text-center">
                        <button type="button" class="buttons btn-dark">Show All Cars</button>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-sm">
            <div class="row">
                <div class="col-12 col-lg-8">
                    <div class="content-main-sm">

                    </div>
                </div>
                <div class="col-12 col-lg-4">
                    <div class="content-main-sm">

                    </div>
                </div>
            </div>
        </div>
        <div class="jumbotron mb-5">
            <div class="container">
                <div class="row gy-3">
                    <div class="col-12">
                        <div class="content-main-jumbo">
    
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-3">
                        <div class="content-main-jumbo-cards">
    
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-3">
                        <div class="content-main-jumbo-cards">
    
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-3">
                        <div class="content-main-jumbo-cards">
    
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-3">
                        <div class="content-main-jumbo-cards">
    
                        </div>
                    </div>
                    <div class="col-12">
                        <div class="content-main-jumbo mb-3">
    
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="container mb-5">
            <div class="row gy-2">
                <div class="col-12">
                    <div class="content-main-bottom">

                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-bottom-cards">
                        
                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-bottom-cards">
                        
                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-bottom-cards">
                        
                    </div>
                </div>
                <div class="col-12 col-md-6 col-lg-3">
                    <div class="content-main-bottom-cards">
                        
                    </div>
                </div>
            </div>
        </div>
        
    </main>
</template>

<style lang="scss" scoped>
.content-main-top-li{
    padding: 25px 0;
    .list-unstyled li{
        font-size: 12px;
        flex-basis: calc(100% / 8);
        max-width: calc(100% / 8);
        flex-grow: 1;
        padding: 15px;
        border: 1px solid black;
        background-color: red;
        text-align: center;
        border-radius: 5px;
        margin: 0 5px;
    }
}

.content-main-top-type{
    width: 100%;
    height: 200px;
    margin-bottom: 20px;
    background-color: red;
    border: 1px solid black;
}

.content-main-top-cars{
    width: 100%;
    height: 250px;
    background-color: red;
    border: 1px solid black;
}

.content-main{
    background-color: red;
    border: 1px solid black;
    .buttons{
        padding: 12px 25px;
        color: #fff;
        background-color: black;
        border: none;
        font-size: 12px;
        font-weight: bold;
    }
}

.container-sm{
    padding: 0 70px;
    margin-bottom: 70px;
    .content-main-sm{
        height: 450px;
        background-color: red;
        border: 1px solid black;
    }

}

.jumbotron{
    padding:50px 0;
    background-image: url('../assets/slider-autocar-6.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    .content-main-jumbo{
        height: 80px;
        background-color: red;
        border: 1px solid black;
    
    }
    .content-main-jumbo-cards{
        height: 300px;
        background-color: red;
        border: 1px solid black;
    }

}

.content-main-bottom{
    height: 150px;
    background-color: red;
    border: 1px solid black;
}

.content-main-bottom-cards{
    height: 300px;
    background-color: red;
    border: 1px solid black;
}



</style>