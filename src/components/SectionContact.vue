<template>
   <section>
      <div class="conteiner">
         <div class="left_form">
            <img src="../assets/image/photo.jpg" />
            <b-button style="width: 12vw; height: 2.4vw; margin: 1vw 0 0 7vw;">Загрузить фото</b-button>
         </div>
         <div class="right_form">
            <div class="group">
               <div>
                  <inputform :labelname="`Фамилия`" style="color: #F8BB10; text-transform: uppercase; font-weight: 900;"></inputform>
                  <inputform :labelname="`Имя`" style="color: #F8BB10; text-transform: uppercase; font-weight: 900;"></inputform>
                  <inputform :labelname="`Отчество`" style="color: #F8BB10; text-transform: uppercase; font-weight: 900;"></inputform>
               </div>
               <div>
                  <inputform :labelname="`Профессия`"></inputform>
               </div>
            </div>
            <hr/>
            <div class="group">
               <div>
                  <inputform :labelname="`Город`" style="flex-direction: column; margin-right: 2vw;"></inputform>
                  <inputform :labelname="`Телефон`" style="flex-direction: column; margin-right: 2vw;"></inputform>
                  <inputform :labelname="`Почта`" style="flex-direction: column;"></inputform>
               </div>
            </div>
         </div>
      </div>   
   </section>
</template>

<script>
import InputForm from "../components/InputForm.vue";

export default {
   name: "SectionContact",
   components: {
      'inputform': InputForm
   }
}
</script>

<style scoped lang="scss">
@import "src/assets/scss/function";
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');

.conteiner {
  display: flex;
  flex-direction: row;

  .left_form {
    background-color: rgba($color: #939393, $alpha: 0.1);
    display: flex;
    flex-direction: column;
    width: vw(500);
    height: vw(1000);

    img {
      margin: vw(300) 0 0 vw(100);
      border-radius: 50%;
      width: vw(300);
      height: vw(300);
    }
  }

   .group {
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 0;

      div {
         width: vw(1100);
      }
   }

  .right_form {
    margin: vw(400) 0 0 vw(150);

    div {
      display: flex;
      justify-content: center;
    }

    hr {
      background: #ececec;
      transition: transform 1.2s ease 0.7s, opacity 1.2s ease 0.7s;
      margin: vw(150) 0 vw(50) 0;
    }
  }
}

</style>