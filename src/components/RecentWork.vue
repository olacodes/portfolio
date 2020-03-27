<template>
<div class="recent-work-container">
    <h2>Recent Work</h2>
    <div>
        <WorkList v-bind:imgs="imgs"/>
    </div>
</div>
</template>

<script>
import WorkList from './WorkList'

export default {
    name: "RecentWork",
    components: {
        WorkList
    },
    data: function () {
        return{
            imgs :[
                {
                    id: 0,
                    name: "Bouncer App",
                    image: "https://res.cloudinary.com/olacode/image/upload/v1585309547/personal/bouncer_xuz9ok.webp", 
                    url: "https://bouncerapp.netlify.com/",
                    description: "This is an  ecommerce application for buying and selling of conputers and phone accesories.",

                },
                {
                    id: 1, 
                    name: "eHealths",
                    image: "https://res.cloudinary.com/olacode/image/upload/v1585310653/portfolio/ehealths1_dz2neo.webp", 
                    url: "https://ehealths.herokuapp.com/",
                    description: "A digital health application system that helps hospitals to collect medical data of their user, visualize  and analyse that data.",
                    
                },
                {
                    id: 2, 
                    name: "Expense App",
                    image: "https://res.cloudinary.com/olacode/image/upload/v1585308929/personal/expense-app_kuyeod.webp", 
                    url: "https://ehealths.herokuapp.com/",
                    description: "An online expense reporting software, made for businesses to automate expense."
                },
                {
                    id: 3, 
                    name: "My Portfolio",
                    image: "https://res.cloudinary.com/olacode/image/upload/v1585311348/portfolio/portfolio1_lvukn9.webp", 
                    url: "https://ehealths.herokuapp.com/",
                    description:"",
                    
                }
            ]

        }
    }
}
</script>


<style scoped>
.recent-work-container{
    margin: 70px 0;
    /* text-align: center; */


}

</style>