<template>
  <div class>
    <h1>{{ msg }}</h1>
    <!-- <router-link :to="{name: 'HelloWorld'}">Hello World</router-link> -->
    <a href="" @click.prevent="toHello">Hello World</a>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      msg: 'Home'
    }
  },
  methods: {
    toHello: function(){
      this.$router.push('/hello_world');
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
