<template>
  <b-container>
    <b-row align-v="center">
      <card v-for="curso in cursos" :key="curso.id" :nome="curso.name"></card>
    
    </b-row>
  </b-container>
</template>

<script>
import Card from '@/components/Card.vue';

export default {
  name: "Home",
  data() {
    return {
      cursos: []
    }
  },
  components: {
    Card
  },
  mounted(){
    this.fetchData();
  },
  methods: {
    async fetchData(){
      const res = await fetch("cursos.json");
      const val = await res.json();
      this.cursos = val;
    }
  }
};
</script>
