<template>
   <ul class="breadcrumbs">

      <li class="breadcrumbs__item">
        <Button class="rounded-lg p-2.5 but-0" @click="back">Назад</Button>
      </li>
      <li class="breadcrumbs__item">
        <NuxtLink to="/" class="breadcrumbs__link">Главная</NuxtLink>
      </li>
      <li class="breadcrumbs__item" v-for="(item, index) in items">
          <template v-if="item.type == 'link'">
            <NuxtLink :to="item.link" class="breadcrumbs__link">{{item.name}}</NuxtLink>
          </template>
          <template v-if="item.type == 'text'">
            {{item.name}}
          </template>
      </li>
    </ul>
</template>

<script>
export default {
  components: {},
  props: {
    items: [],
    back: {
      type: Function,
    },
  },
  data() {
    return {
      
    }
  },
}
</script>

<style scoped>
/* breadcrumbs  */
.breadcrumbs {
  list-style-type: none;
  padding: 0px;
  margin:  0px;
  display: flex;
  align-items: center;
  grid-gap: 10px;
}
.breadcrumbs__item {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  line-height: 18px;
  color: #76767D;
}

.breadcrumbs__item:after {
  content: '/';
  display: inline-block;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  line-height: 18px;
  color: #000000;
  margin-left: 5px;
}

.breadcrumbs__item:first-child:after {
  display: none;
}

.breadcrumbs__item:last-child:after {
  display: none;
}

.breadcrumbs__link {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  line-height: 18px;
  color: #000000;
}

/* breadcrumbs end */

@media only screen and (max-width : 600px) {
  /**/

  .breadcrumbs__item {
    display: none;
  }
  .breadcrumbs__item:first-child,
  .breadcrumbs__item:last-child {
    display: block;
  }
}

</style>