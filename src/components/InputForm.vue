<template>
   <div>
      <label>{{ labelname }}</label>
      <b-input></b-input>
   </div>
</template>

<script>

export default {
   name: 'InputForm',
   props: {
      labelname: { type: String }
   }
}
</script>

<style scoped lang="scss">
   @import "src/assets/scss/function";

   div {
      display: flex;
      flex-direction: row;
      margin: 0 vw(30) vw(40) 0;
      
      label {
         margin: auto vw(15);
      }
   }
</style>