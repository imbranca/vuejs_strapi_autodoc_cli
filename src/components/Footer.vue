<template>
  <footer style="overflow: hidden;">
    <div class="row w-full flex">
      <div class="col-4 col-md-2">
        <div class="brand"><a class="navbar-brand"><img class="logo" src="@/assets/images/logo.png"></a></div>
        <div class="links">
          <div class="icon-links"><a href="https://www.facebook.com/AutoDoc-Peru-108584271589896" target="_blank"
              style="color: white;"><i class="fa fa-facebook-official"></i></a><a
              href="https://wa.me/51981520644?text=Estoy+Interesado%2C+requiero+informaci%C3%B3n+sobre+un+repuesto"
              style="color: white;"><i aria-hidden="true" class="fa fa-whatsapp"></i></a></div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div style="width: 100%; height: 100px;"><img src="@/assets/images/contact.png" alt="" class="contact-image">
        </div>
      </div>
    </div>
  </footer>
</template>
<style>
  footer{
    background-color: #1a1960;
    min-height: 150px;
    padding-left: 50px;
    padding-top: 20px;
    padding-right: 50px;
    color: #eeeeee;
  }
</style>
<script lang="ts">
import { Options, Vue } from 'vue-class-component';

  export default class Footer extends Vue{
  }
</script>