<template>
  <section class="home">
    <div class="container flex">
      <div class="home_col">
        <div class="home_textWrapper text-left">
          <h3>Tu aliado en</h3>
          <h1>Autopartes</h1>
          <div class="font-description">Encuentra repuestos originales y genéricos</div>
        </div>
      </div>
      <div class="home_col home_motor">
        <img class="home_motorImg" src="@/assets/images/Motor.png">
      </div>
    </div>
  </section>
  <section class="product_section">
    <div class="container flex">
      <div class="col-6 flex">
        <div class="product_textWrapper">
          <h2>PRODUCTOS</h2>
          <p class="font-description">Compra y venta segura de productos originales</p>
        </div>
      </div>
      <div class="col-6 flex product_card-container">
        <div class="product_card">
          <img src="@/assets/images/home/Partes_encendido.png" alt="">
          <div class="product_card-title">
            Partes encedido
          </div>
          <div class="product_card-description">
            Motor, Suspencion
          </div>
        </div>
        <div class="product_card">
          <img src="@/assets/images/home/Honda.png" alt="">
          <div class="product_card-title">
            Kit de distribucion
          </div>
          <div class="product_card-description">
            Honda Civic 1.8
          </div>
        </div>
        <div class="product_card">
          <img src="@/assets/images/home/subaru.png" alt="">
          <div class="product_card-title">
            Impreza Legacy Forester
          </div>
          <div class="product_card-description">
            Subaru
          </div>
        </div>
      </div>
    </div>
  </section>
  <section class="brands_section">
    <div class="container flex">
      <div class="col-6 flex">
        <div class="brands_textWrapper">
          <h2>MARCAS
          </h2>
          <p class="font-description">Trabajamos con las mejores marcas <br> Cotiza al instante</p>
        </div>
      </div>
      <div class="col-6 brands_autoBackground">
        <img class="brands_img" src="@/assets/images/marcas.png">
      </div>
    </div>
  </section>
  <section class="faq_section">
    <div class="container flex">
      <div class="faq_textWrapper">
        <h2>PREGUNTAS FRECUENTES</h2>
        <p>Todo lo que necesitas saber de AutoDoc</p>
      </div>
    </div>
  </section>
  <Footer></Footer>
</template>

<style lang="scss">
  .faq{
    &_section{
      height: 600px;
    }
    &_textWrapper{
      position: relative;
      margin: auto;
      margin-top: 20px;
      text-align: left;
    }
  }
  .brands{
    &_section{
      background-color: #ff6c00;
      color: white;
      height: 400px;
    }
    &_autoBackground{
      background-image: url('@/assets/images/auto.png');
      background-position: left;
      position: relative;
    }
    &_img{
      position: absolute;
      left: 0;
      top: 40px;
    }
    &_textWrapper{
      margin: auto;
      position: relative;
      h2{
        position: relative;
        z-index: 100;
        &::before{
          content: '';
          background-image: url('@/assets/images/D.png');
          width: 200px;
          position: absolute;
          display: block;
          height: 300px;
          top: -120px;
          z-index: -1;
        }
      }
      p{
        z-index: 100;
        position: relative;
      }
    }
  }
  .product{
    &_section{
      background-color: #eeeeee;
      height: 600px;
    }
    &_textWrapper{
      margin: auto;
      position: relative;
      h2{
        position: relative;
        z-index: 100;
        &::before{
          content: '';
          background-image: url('@/assets/images/A.png');
          width: 200px;
          position: absolute;
          display: block;
          height: 300px;
          top: -200px;
          z-index: -1;
        }
      }
      p{
        z-index: 100;
        position: relative;
      }
    }
    &_card{
      background-color: white;
      box-shadow: 5px 5px 10px grey;
      border-radius: 10px;
      max-width: 200px;
      max-height: 300px;
      img{
        max-width: 100%;
        border-radius: 10px;
      }
      &-container{
        gap: 20px;
      }
      &-title{
        font-size: 24px;
        font-family: 'PFBulletin', sans-serif;
      }
      &-description{
        font-size: 22px;
      }
      &:nth-child(1), &:nth-child(3){
        margin-top: 100px;
      }
      &:nth-child(2){
        margin-top: 160px;
      }
    }
  }
  .home{
    height: 600px;
    color: white;
    background: linear-gradient(180deg, #1a1960 0%, #0f0e3d 100%);
    .container{
      height: 100%;
    }
    &_textWrapper{
      margin: auto;
    }
    &_col{
      width: 50%;
      height: 100%;
      display: flex;
      flex-direction: column;
    }
    &_motorImg{
      z-index: 10000;
      position: relative;
      margin: auto;
    }
    &_motor{
      position: relative;
      &::before{
        content: '';
        width: 50px;
        height: 100%;
        background-color: #ff6c00;
        position: absolute;
        display: block;
        z-index: 1;
        left: 50%;
      }
      &::after{
        content: '';
        top: 0;
        width: 100px;
        height: 100%;
        background-color: #27265d;
        position: absolute;
        display: block;
        z-index: 0;
        left: 50%;
      }
    }
  }
</style>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import Footer from '@/components/Footer.vue';

@Options({
  components: {
    HelloWorld,
    Footer
  },
})
export default class HomeView extends Vue {}
</script>
