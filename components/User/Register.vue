<template>
    <div class="flex justify-content-center grid grid-nogutter p-6">
        <div class="col-12 md:col-6 bg-blue-300 border-round-md">
            <img class="border-round-lg border-noround-right" src="assets/images/register.png" height="100%" width="100%"/>
        </div>
        <div class="cardForm col-12 md:col-6 border-round-lg border-noround-left">
            <h1 class="m-4 flex justify-content-center align-content-start">Register - <span class="text-blue-400 ml-2 mr-2">RespirAr Hub</span></h1>
            <label class="m-4 flex justify-content-center align-content-start">Welcome to the Intelligent Air Purification System. Register or log in to experience.</label>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>Nome</label>
                <InputText id="emailForm" v-model="name"/>
            </div>
            <div class="formStyle flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>E-mail</label>
                <InputText id="emailForm" v-model="email"/>
            </div>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>Senha</label>
                <InputText id="emailForm" v-model="password"/>
            </div>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>Confirme sua senha</label>
                <InputText id="emailForm" v-model="confirmPassword"/>
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
            name: '',
            email: '',
            password: '',
            confirmPassword: '',
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

.cardForm{
    background-color: rgb(32, 32, 32);
}

</style>