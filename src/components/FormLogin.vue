<template>
    <form @submit.prevent="handleSubmit">
        <div class="form-group">
            <label for="password" class="login-label">RUT</label>
            <div class="input-group mb-3">
                <div class="input-group-prepend">
                    <span class="input-group-text" id="basic-addon1"><AccountOutline/></span>
                </div>
                <input type="text" class="form-control" placeholder="Username" aria-label="Username"
                    aria-describedby="basic-addon1">
            </div>
        </div>
        <div class="form-group">
            <label for="password" class="login-label">Contraseña</label>
            <div class="input-group mb-3">
                <div class="input-group-prepend">
                    <span class="input-group-text" id="basic-addon1"><LockOutline/></span>
                </div>
                <input type="text" class="form-control" placeholder="Username" aria-label="Username"
                    aria-describedby="basic-addon1">
            </div>
        </div>
        <div class="form-group">
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="defaultCheck1">
                <label class="form-check-label" for="defaultCheck1">
                    Default checkbox
                </label>
            </div>
        </div>
        <button type="submit" class="btn btn-primary btn-block mt-3 w-100">
            Iniciar sesión
        </button>
        <button type="submit" class="btn btn-custom btn-block mt-3 w-100">
            Registrarse
        </button>
    </form>
</template>

<script>
import AccountOutline from 'vue-material-design-icons/AccountOutline.vue'
import LockOutline from 'vue-material-design-icons/LockOutline.vue'

export default {
    name: 'FormLogin',
    components:{
        AccountOutline,
        LockOutline
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.input-group-text {
    border-top-left-radius: 4px;
    border-bottom-left-radius: 4px;
    border-top-right-radius: 0px;
    border-bottom-right-radius: 0px;
}

.login-label{
   font-weight: 700; 
   font-size: 19px;
}

.btn{
    border-radius: 8px;
    height: 50px;
}

.btn-custom, .btn-custom:hover{
    border: none;
    background-color: #DCE1FF;
}
</style>