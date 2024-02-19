<template>
  <h3>{{ info }}</h3>
  <p>{{ someInfo }}</p>

  <button type="button" @mouseover ='userData()'>Click me!</button>
</template>

<script>
  export default{
     data(){
      return{
        info: 'Some Title',
        someInfo: 'Some new text'
      }
    },

    methods: {
      userData (){
        this.info = "new title",
        this.someInfo = "new text"
      }
    }
  }
</script>

<style scoped>
h3 {
  font-weight: lighter;
}

p{
  color: rgb(203, 31, 31)
}
</style>
