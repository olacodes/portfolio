<template>
    <div class="card-wrapper">

        <div class="image-container">
            <img v-bind:src="img.image" alt="">
        </div>

        <div class="overlay">
            <h2 class="text">{{img.name}} </h2>
            
        <div class="description">{{img.description}}</div>
        </div>

    </div>
</template>

<script>
export default {
    name: "MyRecentWorkCard",
    props: {
        img: {
            type: Object
        }
    }
}
</script>

<style scoped>
    .card-wrapper{
        /* border: 3px solid red; */
        box-shadow: 3px 3px 6px 6px rgb(196, 203, 204);
        /* width: 70%; */
        position: relative;
    

    }
    .image-container{
        width: 100%;
        height: auto;
    }
    img{
        /* display: block; */
        width: 100%;
        height: 250px;
    }
    .overlay{
        position: absolute;
        bottom: 100%;
        top: 0;
        background-color:  #091f36d7;
        overflow: hidden;
        width: 100%;
        transition: .5s ease;
    }
    .card-wrapper:hover .overlay{
        bottom: 0;
        height: 100%;
    }
    .text {
    white-space: nowrap; 
    color: white;
    font-size: 30px;
    position: absolute;
    overflow: hidden;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
}
.description{
    color: white;
    padding: 14px;
}

</style>