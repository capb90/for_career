<template>
  <div id="app">
    <CardLogin labelSummary="Registrarse">
      <FormResetPassword/>
    </CardLogin>
  </div>
</template>

<script>
import FormResetPassword from './components/FormResetPassword.vue';
import CardLogin from './components/CardLogin';

export default {
  name: 'App',
  components: {
    CardLogin,
    FormResetPassword
  }
}
</script>

<style></style>
