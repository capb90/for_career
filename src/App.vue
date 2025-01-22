<template>
  <div id="app">
    <!-- <CardLogin labelSummary="Registrarse">
      <FormResetPassword/>
    </CardLogin> -->
    <MainLayout>
      <template #header>
        <HeaderLayout />

      </template>
    </MainLayout>
  </div>
</template>

<script>
import HeaderLayout from './components/HeaderLayout.vue';
import MainLayout from './components/MainLayout.vue';


export default {
  name: 'App',
  components: {
    HeaderLayout,
    MainLayout
  }
}
</script>

<style></style>
