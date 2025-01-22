<template>
  <div class="layout-container">
    <!-- Header -->
     <slot name="header"></slot>

    <!-- Main Layout -->
    <div class="d-flex">
      <!-- Sidebar -->
      <aside class="layout-sidebar">
        <!-- menú -->
        <ul class="nav flex-column">
          <li class="nav-item">
            <a class="nav-link active" href="#">Inicio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Opción 1</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Opción 2</a>
          </li>
        </ul>
      </aside>

      <!-- Main Content -->
      <main class="layout-content">
        <h1>Bienvenido al Dashboard</h1>
        <p>Contenido principal...</p>
      </main>
    </div>
  </div>
</template>

<script>


export default {
    name: 'MainLayout',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* Layout Container */
.layout-container {
  padding: 0 165px;
}

/* Header */
.layout-header {
  height: 64px;
  background-color: transparent;
  border-bottom: 1px solid #E5E5E5;
}

.layout-header .dropdown-menu {
  padding: 16px !important;
}

/* Sidebar */
.layout-sidebar {
  width: 200px;
  background-color: transparent;
  padding: 1rem;
  min-height: calc(100vh - 64px);
}

/* Main Content */
.layout-content {
  flex: 1;
  padding: 1rem;
}
</style>