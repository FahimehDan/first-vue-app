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

<!-- Conditional directives in Vue Js -->
<h2 v-if="number===0" >This is a number </h2>
<h2 v-else-if="number < 0" >Number is negative </h2>
<h2 v-else-if="number > 0" >Number is positive </h2>
<h2 v-else >Number is not a numner </h2>

<h2 v-show="isVisible" >Data is visible </h2>
<h2 v-if="isVisible" >Data is visible </h2>

<template v-if="fruitIsVisible"> 
<p>pomme</p>
<p>pomme de terre</p>
<p>mange</p>
</template>





</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      name:'Fahimé',
      count: 0,
      count2: 0,
      number: 'hi',
      isVisible: true,
      fruitIsVisible: true,

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
