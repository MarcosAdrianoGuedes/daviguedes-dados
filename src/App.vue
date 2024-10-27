<script setup>
import HelloWorld from './components/HelloWorld.vue'
import { ref } from 'vue'

// Variáveis reativas para email e senha
const email = ref('')
const password = ref('')

// Funções para manipular o envio do email e senha
const submitEmail = () => {
  console.log("Email enviado:", email.value)
}

const submitLogin = () => {
  console.log("Email Enviado:", email.value)
}

</script>

<template>
  <header>

    <div class="wrapper">
      <HelloWorld msg="DAVI GUEDES - ANALISE DE DADOS" />

      <nav>
        <!-- Formulário de login abaixo dos links -->
        <div class="login-form">
          <h2>Faça seu login</h2>
          <label for="email" required>Email:</label>
          <input type="email" v-model="email" id="email" placeholder="Digite seu email..." class="email" />

          <label for="password">Senha:</label>
          <input type="password" v-model="password" id="password" placeholder="Digite sua senha..." class="password" />

        </div>
        <div class="container">
          <button type="submit" form="login-form" onclick="login-form" class="login-button">ENTRAR</button>
        </div>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}

.login-button {
  border-radius: 12px;
  border: none;
  color: white;
  background-color: #00BD7E;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
}

.email,
.password {
  border-radius: 12px;
  border: none;
  padding: 16px;
}

header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

.login-form {
  margin-top: 20px;
  text-align: center;
  border-radius: 12px;
}

label {
  display: block;
  margin: 10px 0 5px;
}

input {
  margin-bottom: 10px;
  padding: 8px;
  width: 100%;
  max-width: 300px;
}

button {
  margin-bottom: 15px;
  padding: 8px 16px;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-end;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  }


}
</style>
