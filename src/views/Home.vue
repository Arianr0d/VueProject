<template>
   <div class="main_form">
      <mainheader></mainheader>
      <sectioncontact></sectioncontact>

   </div>
</template>

<script>
import MainHeader from '../components/MainHeader.vue'
import SectionContact from '../components/SectionContact.vue'

export default {
  name: "Home",
  components: {
    'mainheader': MainHeader,
    'sectioncontact': SectionContact
  },
};
</script>

<style scoped lang="scss">

.main_form {
   font-family: 'Lato', sans-serif;
   margin: 0;
   padding: 0;
   box-sizing: border-box;
   color: #727272;
   font-weight: 540;
   font-size: vw(16);
}
</style>
