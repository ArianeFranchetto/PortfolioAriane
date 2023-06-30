<script setup>
import Item from './components/Item.vue';
import Footer from './components/Footer.vue';

</script>

<script>
import dados from './dados/Services.json'

export default {
  data() {
    return {
      services: null
    }
  },
  mounted() {
    this.services = dados

  }
}
</script>

<template>
  <div class="card-icon">

    <div class="title">
      
      <h4 class="text-title">Olá! Eu sou Ariane Franchetto, desenvolvedora Front-end.</h4>
      <div class="text">
        <p>Sou desenvolvedora full stack, com foco em front-end, atualmente no 4º semestre da faculdade de sistemas de informação.
           Com meus 27 anos, estou em busca de novas oportunidades no mercado de trabalho para aplicar minha paixão pela programação e contribuir para projetos desafiadores.
Adquiri uma sólida base teórica e prática, trabalhando em projetos que envolvem linguagens como HTML, VUE3, JS e CSS, assim como frameworks modernos como React e Angular.

Minha experiência se estende além do front-end, pois também possuo conhecimentos em back-end, incluindo bancos de dados como SQL.

Sou uma pessoa comunicativa e valorizo o trabalho em equipe.
</p>
      </div>

   
    </div>
 
   <div class="container-img">
    <img class="photo-icon"
     src="https://avatars.githubusercontent.com/u/87048106?s=400&u=8501f7ff454bf492214084006031b3ec986c9c83&v=4"
      alt="photo-icon">
      <h2 class="text-title">Ariane Franchetto</h2>
      <h2 class="text-title">Front-end Developer</h2>

   </div>
  </div>

  <div class="itens">
    <Item v-for="service, index in services" :key="index" :item="service" />
  </div>

  <div>
      <Footer />
    </div>
</template>

<style scoped>
.photo-icon {
  width: 200px;
  border-radius: 100px;
  box-shadow: 12px 13px 31px 8px rgba(0, 0, 0, 0.75);


}

.text-title { 
  color: rgba(0, 0, 0, 0.685);
  margin-top: 15px;
}

.title {
  font-size: 17px;
  display: flex;
  align-items: center;
  flex-direction: column;
  color: rgba(0, 0, 0, 0.685);

}

.container-img {
  display: flex;
  flex-direction: column;
  align-items: center;
  
}

.text {
  display: flex;
  flex-direction: row;
  align-items: center;
  text-align: center;
  width: 600px;
 
}


.card-icon {
  display: flex;
  justify-content: space-evenly;
  flex-direction: row;
  align-items: center;
  color: rgb(221, 233, 244);
  background-image: linear-gradient(10deg, #fddeea 0, #f2d1e1 16.67%, #e2bdd4 33.33%, #cca4c3 50%, #b48cb4 66.67%, #a07baa 83.33%, #8f71a5 100%);
  padding: 10px;
}

.itens {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  background-color: #fff;
  padding-bottom: 100px;

}



@media (max-width: 600px) {
  .photo-icon {
    width: 100px;
  }

  .title {
    font-size: 12px;
  }

  .card-icon {
    display: flex;
    flex-direction: column;
  }

  .text-title {
    font-size: 15px;


  }

}</style>
