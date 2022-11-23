<!--conditional rendering have 4 directives v-if, v-else, v-else-if, v-show-->
<template>
  <h2 v-if="num === 0">The Number is Zero</h2> <!--conditionaly rendering element we use v-if directive (display elements conditionally)-->
  <h2 v-else-if="num < 0">The Number is Negative</h2> <!--conditionaly rendering element we use v-else-if directive-->
  <h2 v-else-if="num > 0">The Number is Positive</h2> <!--conditionaly rendering element we use v-else=if directive-->
  <h2 v-else>The Number is Not Zero</h2> <!--conditionaly rendering element we use v-else directive-->

<!--conditional rendering multiple element -->
  <template v-if="display">
    <h2>abcd</h2>
    <h2>efgh</h2>
    <h2>ijkl</h2>
  </template>

</template>
<script>
export default{
    name :'App',
    data(){
        return {
            num: "hai",
            display: true,
        } 
    }
}
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
