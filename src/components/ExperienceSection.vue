<template>
  <section class="experience" id="my-skills" ref="my-skills">
    <div class="experience-title"><span>My skills</span></div>

    <div class="experience-content">
      <experience-card cardText="Form Builder" @click="goto('https://moutaz-bakier.github.io/')">
         <img src="@/assets/img/form_builder.jpg" />
      </experience-card>
      <experience-card cardText="weather App"  @click="this.$router.push('/weather')">
         <img src="@/assets/img/weatherApp.jpg" />
      </experience-card>
      <experience-card cardText="portfolio met Vuejs (link to github)" @click="goto('https://github.com/M-ayash/portfolio')">
         <img src="@/assets/img/portolio_wit_Vuejs.jpg" />
      </experience-card>
      <experience-card cardText="Wordpress website" @click="goto('https://www.klusbedrijf-direct.nl/')" >
         <img src="@/assets/img/klusbedrijf-direct.png" />
      </experience-card>
      <experience-card cardText="WordPress demo" @click="goto('https://wgv.one-sw.nl/')">
        <img src="@/assets/img/wgv.png" />
      </experience-card>
      <experience-card cardText="WordPress demo" @click="goto('https://xandra.one-sw.nl/')">
        <img src="@/assets/img/xandra.png" />
      </experience-card>
      <experience-card cardText="WordPress demo" @click="goto('https://rentem.one-sw.nl/')">
        <img src="@/assets/img/rentem.png" />
      </experience-card>
      
    </div>
  </section>
</template>

<script>
import ExperienceCard from './ExperienceCard.vue';
export default {
  components: {ExperienceCard},
  methods: {
    goto(url){
      window.location.href =url
    }
  },
};
</script>
<style>
.experience {
  min-height: 90vh;
  height: 100%;
  padding-top: 50px;
}
.experience-title {
  margin: 20px;
}
.experience-title span {
  padding: 10px 100px;
  background-color: rgb(4, 4, 75);
  font-weight: bold;
  color: rgb(245, 244, 237);
  border-radius: 5%;
}
.experience-content {
  display: flex;
  margin: 20px;
  flex-wrap: wrap;
  justify-content: space-around;
}


</style>
