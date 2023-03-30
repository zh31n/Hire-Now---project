<template>
  <div class="header">
    <ModalMessages />
    <div class="container">
      <div class="header_i">
        <div class="mobile_burger">
          <span></span>
          <span></span>
          <span></span>
        </div>
        <NuxtLink to="/" class="logo_m">
          <img src="../assets/images/Logo.svg" alt="logo" class="logo_m">
        </NuxtLink>
        <div class="nav">
          <NuxtLink to="/"><img src="../assets/images/Logo.svg" alt="logo" class="logo"></NuxtLink>
          <NuxtLink to="/" class="navItem">Create a task</NuxtLink>
          <NuxtLink to="/" class="navItem">Find assignments</NuxtLink>
          <NuxtLink to="/myOrders" class="navItem">My orders</NuxtLink>
        </div>
        <div class="icons_h">
          <img src="../assets/images/Язык.svg" alt="">
          <img src="../assets/images/Сообщения.svg" alt="">
          <div class="dropD">
            <img src="../assets/images/bell.svg" style="position: relative;z-index: -1;" alt="">
            <Notifications />
          </div>
          <NuxtLink class="i_pr" to="/Profile">
            <img src="../assets/images/Аватар.svg" alt="">
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ModalMessages from './Modals/ModalMessages.vue';
import ModalChoosePerformer from './Modals/ModalChoosePerformer.vue';
import ModalChoosedPerformer from "~/components/Modals/ModalChoosedPerformer.vue";
import Notifications from './Modals/Notifications.vue';
import OrderInProgress from './Modals/OrderInProgress.vue';
import OfferTask from './Modals/OfferTask.vue';
import CreatedOfferTask from './Modals/CreatedOfferTask.vue';
import OrderNoComplete from "~/components/Modals/OrderNoComplete.vue";



export default {
  components: {OrderNoComplete, Notifications, ModalChoosedPerformer, ModalMessages, ModalChoosePerformer, OrderInProgress, OfferTask, CreatedOfferTask }
}
</script>

<style lang="scss" scoped>

.dropD{
  display: inline-block;
  position: relative;
}
.header {
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed !important;
  background-color: white;
  width: 100%;
  border-bottom: 1px solid #F0F0F0;
  height: 60px;
  padding: 4px;
  // position: relative !important;
  z-index: 1000 !important;
}

.header_i {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.navItem {
  color: #22305F;
  font-size: 14px;
  font-weight: 700;
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 45%;
}

.icons_h {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 17%;
}

.mobile_burger {

  flex-direction: column;
  gap: 4px;

  span {
    width: 25px;
    height: 4px;
    background-color: grey;

  }

  display: none;
}

.logo_m {
  display: none;
}

// MEDIA QUERIES

@media (max-width:768px) {
  .nav {
    width: 50%;
  }

  .icons_h {
    width: 25%;
  }
}

@media (max-width:670px) {
  .nav {
    display: none;
  }

  .logo_m {
    display: block;
    padding-left: 2rem;
  }

  .mobile_burger {
    display: flex;
  }

  .i_pr {
    display: none;
  }

  .icons_h {
    width: auto;
    gap: 10px;
  }
}
</style>
