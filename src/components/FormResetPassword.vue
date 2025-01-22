<template>
    <form @submit.prevent="handleSubmit">
        <div class="form-group">
            <label for="password" class="login-label">RUT</label>
            <div class="input-group mb-3">
                <div class="input-group-prepend">
                    <span class="input-group-text" id="basic-addon1">
                        <AccountOutline />
                    </span>
                </div>
                <input type="text" class="form-control" placeholder="RUT" aria-label="Username"
                    aria-describedby="basic-addon1">
                <small class="help-text">Rut sin puntos, sin guion y sin digito verificador. Ejemplo: 177078393</small>
            </div>
        </div>
        <button type="submit" class="btn btn-primary btn-block mt-3 w-100">
            Recuperar contraseña
        </button>
        <button type="button" class="btn btn-custom btn-block mt-3 w-100">
            Cancelar
        </button>
    </form>
</template>

<script>
import AccountOutline from 'vue-material-design-icons/AccountOutline.vue'

export default {
    name: 'FormResetPassword',
    data() {

        return {
            typeInputPassword: String,
        }
    },
    components: {
        AccountOutline,
    },
    methods: {
        handleSubmit() {
            console.log('EVENT FORM')
        }
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
    background-color: transparent;
}


.login-label {
    font-weight: 700;
    font-size: 19px;
}

.btn {
    border-radius: 8px;
    height: 50px;
}

.btn-custom,
.btn-custom:hover {
    border: none;
    background-color: #DCE1FF;
}

.help-text {
    font-weight: 400;
    font-size: 12px;
}
</style>