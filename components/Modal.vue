<template>
  <transition name="modal-fade">
    <div class="modal-overlay md:px-12" @click="$emit('close-modal')">
      <div class="modal-content md:w-4/5 w-full">
        <div class="modal h-full" @click.stop>
          <slot></slot>  
        </div>
        <div class="close" @click="$emit('close-modal')">x</div>
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  components: {},
  props: {
    show: false
  },
  watch: {
    show: function( val ){
      if ( val ) {
        
      }
    }
  },
  data() {
    return {
    }
  },
  mounted() {

  },
}
</script>

<style scoped>
.modal-overlay {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #000000da;
  z-index: 1000000;
}
.modal-content {
  position: relative;
}
.modal {
  
}
.close {
  cursor: pointer;
  background-color: #fff;
  position: absolute;
  top: 0px;
  right: -10px;
  padding: 1px 6px;
  border-radius: 100%;
}

.modal-fade-enter,
.modal-fade-leave-to {
  opacity: 0;
}
.modal-fade-enter-active,
.modal-fade-leave-active {
  transition: opacity 0.5s ease;
}
</style>