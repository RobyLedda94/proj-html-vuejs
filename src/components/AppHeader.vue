
<script>
export default {
    
}
</script>

<template lang="">
    <header>
        <div class="container">
            <div class="row gx-0">
                <div class="col-12 col-sm-6">
                    <div class="content-header">
                        <!-- logo + ul + icone -->
                    </div>
                </div>
                <div class="col-12 col-sm-6">
                    <div class="content-header">
                        <!-- logo + ul + icone -->
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

header{
    background-color:#fff;
    padding: 10px 0px;
}
.container {
    .content-header{
        height: 75px;
        border: 1px solid black;
        background-color: red;
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