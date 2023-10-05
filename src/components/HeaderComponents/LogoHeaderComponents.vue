<script setup>
import { reactive } from "vue";
import LogoPabuAgro from "../../assets/img/logo.png"

const pabuAgroInfo = reactive({
  logo: LogoPabuAgro,
  name: "PACAEMBU"
})
</script>

<template>
  <div class="logo">
    <div class="logo__box">
      <img class="logo__box__img" :src="pabuAgroInfo.logo" alt="">
      <span class="logo__box__name" v-html="pabuAgroInfo.name"></span>
    </div>
  </div>
</template>

<style scoped>
.logo {
  background-color: #004A35;
  display: flex;
  justify-content: center; 
  align-items: center;
  height: 80px;
  color: #fff;
} 
.logo__box {
  width: 80%;
  display: flex;
  align-items: center;
  gap: 10px;
}

.logo__box__img{
  width: 30px;
}

.logo__box__name{
  font-weight: 700;
  font-size: 20px;
}
</style>
