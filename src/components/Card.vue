<template>
  <div>
    <b-col>
      <b-card 
        :title="nome"
        img-src="https://picsum.photos/600/300"
        img-alt="Curso de VueJS"
        style="max-width: 20rem"
        img-top
        tag="article"
        class="mb-2"
        border-variant="primary"
        header="Curso"
        header-bg-variant="primary"
        header-text-variant="white"
        align="center"
      >
        <b-card-text>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Facere nemo
          alias amet ipsa reiciendis quas cupiditate voluptatem impedit labore
          saepe fuga laboriosam, temporibus, molestias tempora dolore. Repellat
          quasi vero temporibus!
        </b-card-text>
        <b-button variant="primary">Comprar</b-button>
      </b-card>
    </b-col>
  </div>
</template>

<script>
export default {
  props: {
    nome: {
      type: String,
      required: true
    }
  }
};
</script>