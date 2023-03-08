<template>
  <div class="header">
    <Notifications style="display: none;"/>
    <div class="container">
      <div class="header_i">
        <div class="nav">
          <NuxtLink to="/"><img src="../assets/images/Logo.svg" alt="logo" class="logo"></NuxtLink>
          <NuxtLink to="/" class="navItem">Create a task</NuxtLink>
          <NuxtLink to="/" class="navItem">Find assignments</NuxtLink>
          <NuxtLink to="/myOrders" class="navItem">My orders</NuxtLink>
        </div>
        <div class="icons_h">
          <img src="../assets/images/Язык.svg" alt="">
          <img src="../assets/images/Сообщения.svg" alt="">
          <img src="../assets/images/bell.svg" alt="">
          <img src="../assets/images/Аватар.svg" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Notifications from './Modals/Notifications.vue';


export default {
    components: { Notifications }
}
</script>

<style lang="scss" scoped>
.header {
  background-color: white;
  width: 100%;
  border-bottom: 1px solid #F0F0F0;
  height: 60px;
  position: relative !important;
  z-index: 1000 !important;
}

.header_i {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.navItem{
  color: #22305F;
  font-size: 14px;
  font-weight: 700;
}

.nav{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 45%;
}

.icons_h{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 17%;
}
</style>