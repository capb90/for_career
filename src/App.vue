<template>
  <div id="app">
    <CardLogin labelSummary="¿Has olvidado tu contraseña?">
      <FormLogin/>
    </CardLogin>
  </div>
</template>

<script>
import FormLogin from './components/FormLogin';
import CardLogin from './components/CardLogin';

export default {
  name: 'App',
  components: {
    CardLogin,
    FormLogin
  }
}
</script>

<style></style>
