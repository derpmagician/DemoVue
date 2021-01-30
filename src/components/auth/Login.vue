<template>
 <div>
   <form class="login" @submit.prevent="login">
     <h1>Escribe tus datos</h1>
     <label>Email</label>
     <input required v-model="email" type="email" placeholder="tu@correo.pe"/>
     <label>Clave</label>
     <input required v-model="password" type="password" placeholder="Clave"/>
     <hr/>
     <button type="submit">Entra</button>
   </form>
 </div>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      password: ""
    };
  },

  methods: {
    login: function() {
      let email = this.email;
      let password = this.password;
      this.$store
        .dispatch("login", { email, password })
        .then(() => this.$router.push("/"))
        .catch(err => console.log(err));
    }
  }
};
</script>