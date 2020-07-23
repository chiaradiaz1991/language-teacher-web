<template>
    <a @click="scrollTop" v-show="visible" class="bottom-right">
        <slot>
          <img src="../../assets/scrollButton.png" />
        </slot>
    </a>
</template>

<script>
export default {
  data () {
    return {
      visible: false
    }
  },
  methods: {
    scrollTop: function () {
      this.intervalId = setInterval(() => {
        if (window.pageYOffset === 0) {
          clearInterval(this.intervalId)
        }
        window.scroll(0, window.pageYOffset - 50)
      }, 20)
    },
    scrollListener: function () {
      this.visible = window.scrollY > 150
    }
  },
  mounted: function () {
    window.addEventListener('scroll', this.scrollListener)
  },
  beforeDestroy: function () {
    window.removeEventListener('scroll', this.scrollListener)
  }
}
</script>

<style scoped>
.bottom-right {
  position: fixed;
  bottom: 20px;
  right: 20px;
  cursor: pointer;
  animation: appear 1.5s ease-in-out;
}
img {
  box-shadow: 0px 4px 10px rgba(116, 78, 153, 0.2);
  border-radius: 50%;
  margin-bottom: 30px;
  width: 50px;
}
@keyframes appear {
  0% { 
  opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    opacity: 1;
  }
}
@media (min-width: 768px) {
  .bottom-right {
    display: none;
  }
}
</style>