<template>
   <div :class="styleForm">
      <label>{{ labelname }}</label>
      <b-input></b-input>
   </div>
</template>

<script>

export default {
   name: 'InputForm',
   props: {
      labelname: { type: String },
      styleform: {
         type: String,
         default: 'column'
      }
   },
   computed: {
      styleForm() {
         return {
            "flex-direction": this.styleform
         }
      }
   }
}
</script>

<style scoped lang="scss">
   @import "src/assets/scss/function";

   div {
      display: flex;
      flex-direction: column;
      margin-bottom: vw(40);
      
      label {
         margin: auto vw(30);
      }

      b-input {
         align-items: center;
      }
   }
</style>