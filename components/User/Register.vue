<template>
    <div class="flex justify-content-center grid grid-nogutter p-6">
        <div class="col-12 md:col-6">
            <img class="imagemLogo border-round-lg border-noround-right" src="/public/LOGOREGISTER.png" height="100%" width="100%"/>
        </div>
        <div class="cardForm col-12 md:col-6 border-round-lg border-noround-left">
            <h1 class="m-4 flex justify-content-center align-content-start">Register</h1>
            <label class="m-4 flex justify-content-center align-content-start">Welcome to the Intelligent Air Purification System. Register or log in to experience.</label>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>Name</label>
                <InputText id="emailForm" v-model="Name"/>
                <small id="Password-help">Enter your Name.</small>
            </div>
            <div class="formStyle flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>E-mail</label>
                <InputText id="emailForm" v-model="email"/>
                <small id="email-help">Enter your E-mail aderess.</small>
            </div>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>Password</label>
                <InputText id="emailForm" v-model="password"/>
                <small id="Password-help">Enter your Password.</small>
            </div>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>Confirm password</label>
                <InputText id="emailForm" v-model="confirmPassword"/>
                <small id="ConfirmPassword-help">Enter your Password again.</small>
            </div>
            <div class="card flex justify-content-start p-4">
                <Checkbox v-model="checkbox" :binary="true" />
                <label class="pl-2">Log in after registration</label>
            </div>
            <div class="card flex justify-content-center">
                <Button class="buttonLogin w-9 m-4" label="Register"/>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
        Name: '', // Inicializado como string vazia
        email: '',
        password: '',
        confirmPassword: '', // Adicionado
        checkbox: false,
        }
    },
    methods: {
        submitForm() {
            if (this.checkbox) {
            this.$router.push('/user/login');
            }
    }
}
}
</script>

<style scoped>

.cardLogin{
    background-color: transparent;
    border-radius: 0%;
    height: 100%;
    width: 100%;
}
.cardForm{
    background-color: rgb(32, 32, 32);
}
.buttonLogin{

}

</style>