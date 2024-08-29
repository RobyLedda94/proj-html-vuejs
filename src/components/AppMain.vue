

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
                <div class="col-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
                <div class="col-2">
                    <div class="content-main-top-type">

                    </div>
                </div>
            </div>
            <div class="row g-0 mb-3">
                <div class="col-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-3">
                    <div class="content-main-top-cars"></div>
                </div>
            </div>
            <div class="row g-0">
                <div class="col-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-3">
                    <div class="content-main-top-cars"></div>
                </div>
                <div class="col-12">
                    
                </div>
            </div>
        </div>
        
    </main>
</template>

<style lang="scss" scoped>
.content-main-top-li{
    padding: 25px 0;
    .list-unstyled li{
        flex-basis: calc(100% / 8); 
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
    
</style>