<template>
    <div class="select" v-on:blur="open = false">
      <div class="select__name p-2.5" @click="open = !open">{{label}}<span class="select__bold">{{selected.name}}</span></div>
      <div class="select__items" :class="{ 'select__items_open' : open }">
        <div
          v-for="(item, i) of items"
          :key="i"
          @click="
            selected = item;
            open = false;
            $emit('input', item.value);
          "
          class="select__item p-2.5"
        >{{ item.name }}</div>
      </div>
    </div>
</template>

<script>
export default {
  components: {},
  props: {
    items: {
      type: Array,
      required: true,
    },
    default: {
      type: String,
      required: false,
      default: null,
    },
    value: '',
    label: '',
    skey: ''
  },
  data() {
    return {
      selected: this.default
        ? this.default
        : this.items.length > 0
        ? this.items[0]
        : null,
      open: false
    }
  },
  mounted() {
    this.$emit("input", this.selected.value);
  },
}
</script>

<style scoped>
.select {
  cursor: pointer;
  position: relative;
}

.select__name:after {
  content: '';
  display: inline-block;
  background: url("/images/arrow-down-small.png") no-repeat top center;
  width: 15px;
  height: 9px;
}

.select__name {
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    color: #989999;
    position: relative;
    /*padding: 7px 14px;*/
    display: flex;
    align-items: center;
    gap: 10px;
    width: 100%;
    background: #fff;
    justify-content: space-between;
    border: 1px solid #989999;
    border-radius: 10px;
}

.select__items {
  position: absolute;
  left: 0px;
  right: 0px;
  top: 100%;
  border-radius: 10px;
  overflow: hidden;
  max-height: 0px;
  z-index: 100;
  background: #fff;
}

.select__item {
  /*padding: 7px 14px;*/
  border-bottom: solid #9899992e 1px;
  
}
.select__item:last-child {
  border: 0px;
}
.select__item:hover {
  background: #f8f8f8;
}

.select__items.select__items_open {
  max-height: 500px;
  border: 1px solid #989999;
}

.select__bold {
  color: #000;
}


</style>