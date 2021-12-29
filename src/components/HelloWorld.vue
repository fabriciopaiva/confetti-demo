<template>
  <main>
  </main>
</template>

<script>
  import Vue from 'vue'
  import VueConfetti from 'vue-confetti'

  Vue.use(VueConfetti)

  export default {
    methods: {
      confettis() {
        var b = true; 
        if (b) {
          this.$confetti.start();
          setTimeout(() => {  this.$confetti.stop(); }, 2000);
        }
      }
    },

    mounted() {     
      this.confettis();
    }
  }
</script>