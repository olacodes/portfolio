// Blue Popsicle: #00458B
// Light Green: #3FD2C7
// Light Grey: #99DDFF
// Grey Blue Leaf: #091f36

<template>
  <div id="app">
    <NavBar />
    <div class="content-container">
      <Hero heroprop='Full-Stack Developer & Mentor'/>
      <RecentWork/>
    </div>
  </div>
</template>

<script>

const NavBar = () => import ('./components/NavBar')
const Hero = () => import ('./components/Hero')
const RecentWork = () => import ('./components/RecentWork')

export default {
  name: 'App',

  components: {
    // HelloWorld, 
    NavBar,
    Hero,
    RecentWork
  }
  
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #00458B;
  /* margin-top: 60px; */
  /* background-color: #091f36; */
}
.content-container{
  margin: 0 20px;
}
@media screen and (min-width: 900px) {
  .content-container{
    width: 900px;
    margin-left: auto;
    margin-right: auto;
    /* background-color: #00458B; */
  }
}
</style>
