<template>
  <div class="conteiner">
    <div class="left_form">
      <img src="../assets/image/photo.jpg" />
      <b-button>+ Загрузить фото</b-button>
    </div>
    <div class="right_form">
      <div>
        <inputform
          :labelname="`Фамилия`"
          :widthbutton="widthbtntype1"
        ></inputform>
        <inputform :labelname="`Имя`" :widthbutton="widthbtntype1"></inputform>
        <inputform
          :labelname="`Отчество`"
          :widthbutton="widthbtntype1"
        ></inputform>
      </div>
      <div>
        <inputform
          :labelname="`Профессия`"
          :widthbutton="widthbtntype2"
          :styleform="`column`"
        ></inputform>
      </div>
      <div>
        <inputform
          :labelname="`Город`"
          :widthbutton="widthbtntype2"
        ></inputform>
        <!--<inputform :labelname="`Телефон`" :widthbutton="widthbtntype2" style="flex-direction: column;"></inputform>
            <inputform :labelname="`Почта`" :widthbutton="widthbtntype2"    style="flex-direction: column;"></inputform>-->
      </div>
      <hr />
    </div>
  </div>
</template>

<script>
import InputForm from "../components/InputForm.vue";

export default {
  name: "Home",
  components: {
    inputform: InputForm,
  },
};
</script>

<style scoped lang="scss">
@import "src/assets/scss/function";

.conteiner {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  display: flex;
  flex-direction: row;

  .left_form {
    background-color: rgba($color: #939393, $alpha: 0.1);
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: vw(500);

    img {
      border-radius: 50%;
      width: vw(300);
      height: vw(300);
    }
  }
  .right_form {
    div {
      display: flex;
      justify-content: center;
    }

    hr {
      background: #ececec;
      transition: transform 1.2s ease 0.7s, opacity 1.2s ease 0.7s;
    }
  }
}
</style>

<!--<template>
   <div class="container">
      <form action="">
         <div class="left_form">
            <img src="../assets/image/photo.jpg">
            <b-button>+ Загрузить фото</b-button>
         </div>
         <div class="right_form">
            <div>
               <label for="">Фамилия</label>
               <b-input></b-input>
               <label for="">Имя</label>
               <b-input></b-input>
               <label for="">Отчество</label>
               <b-input></b-input>
            </div>
            <div>
               <label for="">Профессия</label>
               <b-input></b-input>
            </div>
            <div>
               <label for="">Дата рождения</label>
               <b-input></b-input>
               <label for="">Образование</label>
               <b-input></b-input>
            </div>
            <hr>
            <div>
               <label for="">Город</label>
               <label for="">Телефон</label>
               <label for="">Почта</label>
            </div>
            <div>
               <b-input></b-input>
               <b-input></b-input>
               <b-input></b-input>
            </div>
            <div><label for="">О себе</label></div>
            <div>
               <textarea name="" id="" cols="30" rows="10"></textarea>
            </div>
         </div>
      </form>
   </div>
</template>

<script>

export default {
  name: 'Home'
}
</script>

<style scoped lang="scss">
   @import "src/assets/scss/function";

   .container {
      
      margin: 0;
      padding: 0;

      form {
         display: flex;
         flex-direction: row;
         height: vw(950);
   
         .left_form {
            width: vw(600);
            justify-content: flex-start;
            background-color: #fbfbfb;

            img {
               border-radius: 50%;
               width: vw(300);
               height: vw(300);
               margin-top: vw(200);           
            }

            b-button {
               margin-top: vw(10);
            }

         }

         .right_form {
            width: auto;
            justify-content: center;
            margin: vw(200) vw(50);

            div {
               display: flex;
               justify-content: center;
               margin-bottom: vw(40);

               label {
                  margin: auto vw(20);
               }
               
               b-input {
                  width: vw(100);

               }
            }

            hr {
               background: #ececec;
               transition: transform 1.2s ease 0.7s, opacity 1.2s ease 0.7s;
            }
         }
      }
   }

   textarea {
      width: vw(650);
      height: vw(200);
   }

   
</style>-->
