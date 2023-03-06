<template>
    <label class="input-checkbox">
        <input type="checkbox" name="" class="input-checkbox__input" v-model="checked">
        <span class="input-checkbox__active">✔</span>
    </label>
</template>

<script>
export default {
  components: {},
  props: {
    value: {
      required: true,
    }
  },
  data() {
    return {
      checked: false
    }
  },
  watch: {
    checked: function( val ) {
      this.$emit('input', val);
    }
  },
  methods: {
  },
  mounted() {
    this.checked = this.value
  }
}
</script>

<style scoped>
.input-checkbox {
  display: inline-block;
  width: 22px;
  height: 22px;
  background: #D9D9D9;
  border-radius: 4px;
  position: relative;
  overflow: hidden;
  cursor: pointer;
  outline: none;
}

.input-checkbox__input:checked ~ .input-checkbox__active {
  display: block;
}

.input-checkbox__active {
  color: #fff;
  position: absolute;
  left: 0px;
  top: 0px;
  width: 100%;
  height: 100%;
  background: #92E6D6;
  text-align: center;
  line-height: 22px;
  display: none;
  outline: none;
}
.input-checkbox__input {
  height: 0px;
  width: 0px;
}
</style>