<template>
  <div class="hero-container">
    <h1 class="pt-5">{{ heroprop }}</h1>
    <p class="py-2">
      I design and code beautifully simple things, and I love what I do.
    </p>
    <div class="img-container mt-5 py-1">
      <img
        src="https://res.cloudinary.com/olacode/image/upload/w_1000,c_fill,ar_1:1,g_auto,r_max,bo_5px_solid_white,b_rgb:262c35/v1583016760/personal/sodiq_1_xorws5.jpg"
        alt="sodiq img"
      />
    </div>
    <div class="about-me pt-3">
    <h2>Hi, I'm Sodiq. Nice to meet you</h2>
    <p class="about__me__para">
      Since beginning my jouney as a software developer, I have done remote work
      for agencies, consulted for startups and collaborate with talented people
      to create software solutions for business and consumer use. I am quietly
      confident naturally curious and perpetually workin on improving myself.
    </p>

    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
  props: {
    heroprop: {
      type: String,
      required: true,
    }
  }
};
</script>

<style scoped>
h1 {
  text-align: center;
}
.img-container > img {
  width: 230px;
  height: 50%;
  border-radius: 70%;
}
.about__me__para{
    /* max-width: 700px; */
    margin: auto;
    text-align: justify;
    margin-top: 20px;

}
</style>
