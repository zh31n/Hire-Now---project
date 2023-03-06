<template>
    <div class="switcher switcher_w">
        <a href="" class="switcher__but" @click.prevent="action('minus')">-</a>
        <span  class="switcher__value">
          <input type="number" v-model="value">
        </span>
        <a href="" class="switcher__but" @click.prevent="action('plus')">+</a>
    </div>
</template>

<script>
export default {
  components: {},
  props: {
    value: {
      required: true,
    },
    min: {
      type: Number,
      required: false,
      default: 0,
    },
    max: {
      type: Number,
      required: false,
      default: 0,
    },
    maxMsg: '',
    minMsg: '',
  },
  data() {
    return {
    }
  },
  watch: {
    value: function (val) {
      this.$emit('input', val);
    }
  },
  methods: {
    action( action ) {
      this.value = parseInt(this.value, 10)
      if ( action == 'minus' ) {
        this.value = this.value - 1
        if ( this.value <= 0) this.value = this.min
      }
      if ( action == 'plus' ) {
        this.value = this.value + 1

        if ( this.max > 0 ) {
          if ( this.value > this.max ) {
            this.value = this.max
            if ( this.maxMsg ) {
              this.$toast.warning( this.maxMsg )
            }
            
          }
        }

      }
    }
  }
}
</script>

<style scoped>
/* Chrome, Safari, Edge, Opera */
input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}

/* this is for Firefox */
input[type=number] {
  -moz-appearance: textfield;
}

.switcher {
  width: 90px;
  height: 40px;
  background: #F7F7FA;
  border-radius: 10px;

  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 18px;
  color: #000000;

  display: flex;
  text-align: center;
  align-items: center;
      
}

.switcher.switcher_w {
  background: #fff;
}
.switcher__but {
  padding: 0px 7px;
}
.switcher__value {
  flex-grow: 3;
}

.switcher__value input {
  width: 100%;
  text-align: center;
}

</style>