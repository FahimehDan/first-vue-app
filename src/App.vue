<template>
<p>{{greeting}} {{name}}</p>
<p v-text="question"> </p>
<p v-html="htmlData" :id="id" :class="id" :style="style"></p>

</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      name:'Fahimé',
      greeting:'Salut',
      question:'Comment vas-tu ?',
      htmlData: '<b> Il fait beau !</b>',
      id: 'new',
      style: {
        color:'red',
        backgroundColor: 'green',
      }
    }
  }
}
</script>

<style>
#app {
  
}
</style>
