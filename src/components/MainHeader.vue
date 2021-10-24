<template>
   <header>
      <div class="header_section logo">Summary</div>
      <div class="header_section right_section">
         <div><a href="">контактные данные</a></div>
         <div><a href="">о себе</a></div>
         <div><a href="">ещё что-то</a></div>
      </div>
   </header>
</template>

<script>

export default {
   name: 'MainHeader'
}

</script>

<style scoped lang="scss">
@import "src/assets/scss/function";
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');

   header {
      display: flex;
      font-family: 'Lato', sans-serif;
      font-weight: bold;

      height: 50px;
      background-color: #727272;
   }

   .logo {
      color: #F8BB10;
      font-size: 30px;
      width: vw(500);
      
      text-transform: uppercase;
   }

   .header_section {
      display: flex;
      align-items: center;
      justify-content: center;

      div {

         a {
            text-decoration: none;
            color: white;
            padding: 0 vw(70) 0 0;
         }

         a:hover {
            color: #F8BB10;
         }
      }
   }

   .right_section {
      padding-left: vw(450);
   }

</style>