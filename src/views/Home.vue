<template>
  <div class="conteiner">
    <div class="left_form">
      <img src="../assets/image/photo.jpg" />
      <b-button>+ Загрузить фото</b-button>
    </div>
    <div class="right_form">
      <div>
        <inputform :labelname="`Фамилия`"></inputform>
        <inputform :labelname="`Имя`"></inputform>
        <inputform :labelname="`Отчество`"
        ></inputform>
      </div>
      <div>
        <inputform :labelname="`Профессия`" :styleform="`column`"></inputform>
      </div>
      <div>
        <inputform :labelname="`Город`"></inputform>
        <!--<inputform :labelname="`Телефон`" style="flex-direction: column;"></inputform>
         <inputform :labelname="`Почта`" style="flex-direction: column;"></inputform>-->
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
