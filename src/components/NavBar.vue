
<template>
    
    <div>
    <b-navbar id='nav' toggleable="sm" type="dark">
        <b-navbar-brand href="#">OS</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
            <b-nav-text class="pr-4 ">Mentorship</b-nav-text>
            <b-button size="sm" class="px-4 text-white" variant="outline-primary" type="text">Say Hello</b-button>
        </b-navbar-nav>
        </b-collapse>
    </b-navbar>
    </div>
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style scoped>
#nav{
    background-color: #00458B !important
}
</style>
