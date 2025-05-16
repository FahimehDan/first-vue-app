<template>
<p>{{greeting}} {{name}}</p>
<p v-text="question"> </p>
<p v-html="htmlData" :id="id" :class="id" :style="style"></p>
<button v-on:click="name='Pierre'">Change le prénom</button>

<!-- Counter App -->
<h2> {{count}} </h2>
<button @click="count += 1">Add</button>
<button @click="count -= 1">Sub</button>

<!-- Counter App 2 -->
<h2> {{count2}} </h2>
<button @click="increment">Add</button>
<button @click="decrement(2)">Sub</button>



</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      name:'Fahimé',
      count: 0,
      count2: 0,

      greeting:'Salut',
      question:'Comment vas-tu ?',
      htmlData: '<b> Il fait beau !</b>',
      id: 'new',
      style: {
        color:'red',
        backgroundColor: 'green',
      }
    }
  },
  methods:{
    increment(){
       this.count2 += 1
    },
    decrement(num){
      this.count2 -= num
    }
  }
}
</script>

<style>
#app {
  
}
</style>
