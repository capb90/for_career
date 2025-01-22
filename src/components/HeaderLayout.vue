<template>
    <header class="layout-header">
        <div class="d-flex justify-content-between align-items-center h-100 px-3">
            <!-- Logo -->
            <div class="logo">
                <img alt="logo" src="../assets/logo-app.svg" />
            </div>

            <!-- Dropdown -->
            <div class="dropdown">
                <b-dropdown size="lg" variant="link" toggle-class="text-decoration-none" no-caret>
                    <template #button-content>
                        <button class="btn btn-link text-dark dropdown-toggle" type="button" aria-haspopup="true"
                            aria-expanded="false">
                            Mi Perfil
                        </button>

                       <!--  <b-button variant="outline" class="btn btn-link text-dark dropdown-toggle">
                            <b-icon icon="power" aria-hidden="true"></b-icon> Logout
                        </b-button> -->
                    </template>
                    <b-dropdown-item href="#">Action</b-dropdown-item>
                    <b-dropdown-item href="#">Another action</b-dropdown-item>
                    <b-dropdown-item href="#">Something else here...</b-dropdown-item>
                </b-dropdown>
            </div>
        </div>
    </header>
</template>

<script>
import AccountCircleOutline from 'vue-material-design-icons/AccountCircleOutline.vue'

export default {
    name: 'HeaderLayout',
    comments:{
        AccountCircleOutline
    }
}
</script>

<style scoped>
/* Header */



.logo img {
    width: 58.33px;
}

.layout-header {
    height: 64px;
    background-color: transparent;
    border-bottom: 1px solid #E5E5E5;
}

.layout-header .dropdown-menu {
    padding: 16px !important;
}
</style>