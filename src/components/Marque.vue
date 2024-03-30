<template>
    <div class="carusel">
        <Vue3Marquee :direction="'reverse'" :animateOnOverflow="true" :duration="24">
        <img src="@/assets/main/carusel_1.svg" alt="">
        <img src="@/assets/main/carusel_2.svg" alt="">
        <img src="@/assets/main/carusel_3.svg" alt="">
        <img src="@/assets/main/carusel_1.svg" alt="">
        <img src="@/assets/main/carusel_2.svg" alt="">
        <img src="@/assets/main/carusel_3.svg" alt="">
        <img src="@/assets/main/carusel_4.svg" alt="">
        <img src="@/assets/main/carusel_5.svg" alt="">
        <img src="@/assets/main/carusel_6.svg" alt="">
        <img src="@/assets/main/carusel_7.svg" alt="">
        <img src="@/assets/main/carusel_8.svg" alt="">
        <img src="@/assets/main/carusel_9.svg" alt="">
        <img src="@/assets/main/carusel_10.svg" alt="">
        <img src="@/assets/main/carusel_11.svg" alt="">
        <img src="@/assets/main/carusel_12.svg" alt="">
        <img src="@/assets/main/carusel_13.svg" alt="">
        <img src="@/assets/main/carusel_14.svg" alt="">
        <img src="@/assets/main/carusel_15.svg" alt="">
        <img src="@/assets/main/carusel_16.svg" alt="">
        <img src="@/assets/main/carusel_17.svg" alt="">
  </Vue3Marquee>
    </div>
</template>

<script>
import { Vue3Marquee } from 'vue3-marquee'
export default {
    components: {
    Vue3Marquee,
  },
}
</script>

<style scoped>
 .carusel{
    /* border: 1px solid; */
    width: 100%;
    border-bottom: 2px solid;
    overflow: hidden;
    display: flex;
    align-items: center;
    gap: 30px;
}
.carusel img{
   display: block;
   width: 100%; 
   /* flex: 1 1 10rem; */
    height: 150px;
    margin: 0 20px;
   margin-bottom: 0;
}

@media (max-width: 768px){
    .carusel img{
    height: 100px;
}
}
@media (max-width: 428px){
    .carusel img{
    height: 80px;
    margin: 0 10px;
}
}
@media (max-width: 375px){
    .carusel img{
    height: 70px;
    margin: 0 0px;
}
}
</style>