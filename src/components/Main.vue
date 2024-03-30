<template>
  <div class="main_container">
    <div class="main_logo">
      <img src="@/assets/main/photo.png" alt="" />
    </div>
    <div class="main_text">
      <a href="#">@elmirelle_eth | founder of Cloudy Nowhere</a>
      <span>
        Cloudy Hi. I'm Elmirelle, a graphic designer. I made up this world by
        accident, and these little faceless creatures were liked by the NFT
        community.
        <br /><br />
        Every new Cloudy face was hand drawn, all NFTs are already sold out,
        every Cloudy has an owner who doesn't want to give it to anyone.
        <br /><br />
        We are now preparing a collection of 3,000 NFTs. So you can find your
        favorite to show you where that mysterious Cloudy Nowhere is. We'll see
        you there. Cloudy welcome...
      </span>
    </div>

    <ul class="main_btn">
      <li>
        <a href="#"><img class="og_img" src="@/assets/home/og.svg" alt="" /></a>
      </li>
      <li>
        <a href="#"
          ><img class="cstm_img" src="@/assets/home/cstm.svg" alt=""
        /></a>
      </li>
    </ul>

    <img
      class="ducg animated-element"
      @mouseover="isHovered = true"
      @mouseleave="isHovered = false"
      :class="{ animate: isHovered }"
      src="@/assets/main/duck.svg"
      alt=""
    />
    <img class="cloud3" src="@/assets/main/cloud3.svg" alt="" />

  </div>
</template>

<script>
import "animate.css";
export default {
  data() {
    return {
      isHovered: false, // isHovered degan muhit o'zgaruvchisini qo'shamiz
    };
  },
};
</script>

<style scoped>
.animated-element {
  transition: transform .3s ease;
}
.animate {
  transform:rotate(-40deg);
}

.main_container {
  position: relative;
  padding: 0 60px;
  max-width: 1130px;
  margin: 100px auto 0;
}

.main_logo {
  width: fit-content;
  margin: 0 auto;
}

.main_logo img {
  width: 100px;
}

.main_text a {
  display: block;
  margin: 15px auto;
  text-align: center;
  font-size: 15px;
  font-weight: 600;
  color: #000;
  font-family: Arial, Helvetica, sans-serif;
}
.main_text span {
  display: block;
  color: #000000;
  font-size: 15px;
  font-family: "TildaSans", Arial, sans-serif;
  line-height: 20px;
  font-weight: 400;
  max-width: 550px;
  margin: 0 auto;
  text-align: center;
}
.main_btn {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 40px auto;
  gap: 10px;
}
.og_img {
  max-width: 240px;
}
.cstm_img {
  max-width: 210px;
}
.ducg {
  position: absolute;
  top: 10%;
  left: 6%;
  width: 60px;
}
.ducg :hover {
  /* transform: translate(20deg);
  left: 20px; */
}
.cloud3 {
  position: absolute;
  top: 15%;
  right: 5%;
  width: 120px;
  animation: clound 4s infinite;
}
@keyframes clound {
  0%,
  100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-15px);
  }
}

@media (max-width: 960px) {
  .main_container {
    padding: 0 60px;
    margin: 30px auto 0;
  }
  .og_img {
    max-width: 220px;
  }
  .cstm_img {
    max-width: 190px;
  }

  .ducg {
    position: absolute;
    top: 6%;
    left: 20%;
    width: 40px;
  }
  .cloud3 {
    position: absolute;
    top: 9%;
    right: 20%;
    width: 90px;
  }
}
@media (max-width: 600px) {
  .main_container {
    padding: 0 60px;
    margin: 60px auto 0;
  }

  .main_text a {
    font-size: 13px;
  }
  .main_text span {
    font-size: 13px;
  }

  .og_img {
    max-width: 160px;
  }
  .cstm_img {
    max-width: 140px;
  }

  .ducg {
    position: absolute;
    top: 6%;
    left: 10%;
    width: 40px;
  }
  .cloud3 {
    position: absolute;
    top: 9%;
    right: 10%;
    width: 90px;
  }
}
@media (max-width: 450px) {
  .main_text a {
    font-size: 10px;
  }
  .main_text span {
    font-size: 10px;
  }
}
@media (max-width: 375px) {
  .main_container {
    padding: 0 60px;
    margin: 0 auto;
  }
  .og_img {
    max-width: 140px;
  }
  .cstm_img {
    max-width: 120px;
  }

  .ducg {
    position: absolute;
    top: 6%;
    left: 10%;
    width: 30px;
  }
  .cloud3 {
    position: absolute;
    top: 9%;
    right: 10%;
    width: 60px;
  }
}
</style>