<template>
    <div class="flex justify-content-center grid p-6">
        <div class="col-12 md:col-6 bg-blue-300 border-round-md">
            <img class="border-round-lg border-noround-right" src="assets/images/login.png" height="100%" width="100%"/>
        </div>
        <div class="cardForm col-12 md:col-6 border-round-lg border-noround-left">
            <h1 class="m-4 flex justify-content-center align-content-start">Login - <span class="text-blue-400 ml-2 mr-2">RespirAr Hub</span></h1>
            <label class="m-4 flex justify-content-center align-content-start">Welcome to the Intelligent Air Purification System. Register or log in to experience.</label>
            <div class="formStyle flex flex-column gap-2 p-4">
                <label>Nome de Usuário ou E-mail</label>
                <InputText id="emailForm" v-model="email"/>
            </div>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>Senha</label>
                <InputText id="emailForm" v-model="password"/>
            </div>
            <div class="card flex justify-content-center flex-column align-items-center">
                <Button class="buttonLogin w-9 m-4" label="Sign in" />
                <Divider align="center" type="dotted">
                    <b>OU</b>
                </Divider>
                <div class="flex justify-content-center align-items-center mt-4">
                    <i class="pi pi-google"></i> <span class="ml-2 cursor-pointer">- Entrar com o Google</span>
                </div>
                <div class="mt-5">
                    <span>Novo por aqui?</span> <a class="text-blue-400 underline cursor-pointer">Criar uma conta agora</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default{
        data(){
            return{
                email:null,
                password:null
            }
        }
    }
</script>

<style scoped>

.cardForm{
    background-color: rgb(32, 32, 32);
}


</style>