<template>
    <h2> Hello world </h2>
    <h3> Hello {{name}} </h3>
    <h3> Hello {{propesName}} </h3>


</template>
 <<script>
 export default {
     name: 'Greet',
     props: ['name']
 }
 </script>