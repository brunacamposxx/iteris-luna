<template>
  <div class="teste-evento">
    <!-- <p>{{ mensagem }}</p> -->
    <p v-if="valida" @click="deixarMinuscula">{{mensagem}}</p>
    <p v-else @click="deixarMaiuscula">{{mensagem}}</p>
  
	</div>
</template>

<script>
export default {
  name: 'TesteEvento',
  data() {
    return {
      mensagem: 'O rato roeu a roupa do rei de Roma',
			valida: true
    }
  },
  methods: {
    deixarMaiuscula() {
      this.mensagem = this.mensagem.toUpperCase();
			this.valida = false;
    },
		deixarMinuscula() {
			this.mensagem = this.mensagem.toLowerCase();
			this.valida = true;
		}
  }
}
</script>