<template>
  <div>
    <!-- <pre>
    {{ $route }}
    </pre> -->

    {{ $route.params.id }}
    Usuário

    <button @click="login()">Login</button>
  </div>
</template>

<script>
export default {
  created() {
    // $route tem dados da rota atual
    console.log(this.$route);

    // $router tem funcionalidades para o roteamento
    console.log(this.$router);
  },

  methods: {
    login() {
      // Ajax login
      this.$router.push("/about");
      console.log("chegou");
    },
  },
};
</script>

<style></style>
