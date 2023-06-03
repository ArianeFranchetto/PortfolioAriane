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
    <img class="photo-icon" src="https://camo.githubusercontent.com/5ff76b74ed4be2e2b0a7778ded89b3c510b292db4e73f6ddb5f098dfb63fdb47/68747470733a2f2f6d656469612e646973636f72646170702e6e65742f6174746163686d656e74732f3732353133383937323930303332373432342f3930373435363639373637393838383338342f7069636173696f6e2e636f6d5f65393035386464376633323036333132373533633934333863363033386131302e676966"
      alt="photo-icon">
      <div class="title">
        <h1>Ariane Franchetto</h1>
      <h2>Front-end Developer</h2>
      <p>descrição descriçãodescriçãodescrição descriçãodescriçãodescriçãodescriçãovvdescrição descrição descriçãodescriçãov  descrição descriçãodescrição</p>
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
  box-shadow: 12px 13px 31px 8px rgba(0,0,0,0.75);

}

.title {
  font-size: 17px;
  display: flex;
  align-items: center;
  flex-direction: column;
}
.card-icon {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  color: rgb(221, 233, 244);
}

.itens {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;

}



@media ( max-width: 600px ) {
    .photo-icon{
        width: 100px;
    }
    .title{
      font-size: 12px;
    }
}
</style>
