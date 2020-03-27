<template>
    <div class="recent-work-list-container">
        <div v-for="img in imgs" :key="img.id" class="recent-work-list">
            <a :href="img.url" target="_blank">
                <RecentWorkCard v-bind:img="img"/>
            </a>
        </div>
    </div>
</template>


<script>

import RecentWorkCard from './RecentWorkCard'

export default {
    name: "WorkList",
    components: {
        RecentWorkCard
    },
    props: {
        imgs: {
            type: Array
        }

    }
}
</script>

<style scoped>
    .recent-work-list{
        margin: 30px auto 0 auto;
        padding: 8px;

        /* border: 5px solid red; */
    }
    .recent-work-list-container{
        /* border: 3px solid greenyellow; */
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }
    @media screen {
        .recent-work-list{
            width: 430px;
        }
    }
</style>