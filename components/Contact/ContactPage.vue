<template>
    <div class="flex justify-content-center grid grid-nogutter p-6">
        <div class="col-12 md:col-6 bg-blue-300 border-round-md">
            <img src="/public/Contac.png" width="100%">
        </div>
        <div class="cardForm col-12 md:col-6 border-round-lg border-noround-left">
            <h1 class="m-4 flex justify-content-center align-content-start">Vamos conversar ! - <span class="text-blue-400 ml-2 mr-2">RespirAr Hub</span></h1>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label class="pt-3 px-0" for="FullName">Nome Completo</label>
                <InputText class="" id="username" v-model="fullName" aria-describedby="username-help" />
            </div>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label class="pt-5 px-0-3" for="Email">E-mail</label>
                <InputText class="" id="email" v-model="email" aria-describedby="email-help" />
            </div>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label class="pt-5 px-0-3" for="Message">Mensagem</label>
                <div class="pt-3 px-0-3" id="editor" contenteditable> </div>
            </div>
            <div class="flex justify-content-end gap-2 pr-4 pb-4 pl-4">
                <Button label="Enviar mensagem" class="w-4"/>
            </div>
        </div>
    </div>
    <Divider align="center" type="dotted">
        <b>Other media</b>
    </Divider>
    <div class="grid flex justify-content-center">
        <div class="cardContact col-12 md:col-3">
            <br>
            <i class="pi pi-instagram flex justify-content-center" style="font-size: 3.0rem"></i>
            <h1 class="flex justify-content-center">Instagram</h1>
            <div class="cardInstagram flex justify-content-center mt-8">
                <p>@RespirarContact</p>
            </div>
            <p class="flex justify-content-center">OR</p>
            <div class="cardInstagram flex justify-content-center">
                <p>@RespirarInstagram</p>
            </div>
        </div>

        <div class="cardContact col-12 md:col-3">
            <br>
            <i class="pi pi-whatsapp flex justify-content-center" style="font-size: 3.0rem"></i>
            <h1 class="flex justify-content-center">Whatsapp</h1>
            <div class="cardWhatsaap flex justify-content-center mt-8">
                <p class="p-2">(19)99999-9999.</p>
            </div>
            <p class="flex justify-content-center">OR</p>
            <div class="cardWhatsaap flex justify-content-center">
                <p>(19)101010-1010.</p>
            </div>
        </div>

        <div class="cardContact col-12 md:col-3">
            <br>
            <i class="pi pi-envelope flex justify-content-center" style="font-size: 3.0rem"></i>
            <h1 class="flex justify-content-center">E-mail</h1>
            <div class="cardEmail flex justify-content-center mt-8">
                <p>RespirAr@gmail.com</p>
            </div>
            <p class="flex justify-content-center">OR</p>
            <div class="cardEmail flex justify-content-center">
                <p>RespirAr@hotmail.com.br</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
data() {
  return {
    fullName: '',
    email: '',
    message: ''
  };
}
}
</script>

<style scoped>

.cardForm{
    background-color: rgb(32, 32, 32);
}


.Titulo {
  font-size: 5rem;
  color: white;
  text-align: center;
}
.card {
  background-color: rgb(32, 32, 32);
  border-radius: 7px;
  padding: 20px;
  margin: 10px;
  color: white;
}
#editor {
  border: 1px solid rgb(32, 32, 32);
  background-color: rgb(26, 26, 26);
  min-height: 200px;
  overflow: auto;
  padding: 10px;
  color: white;
  border-radius: 7px;
}
#username{
    background-color: rgb(26, 26, 26);
}
#email{
    background-color: rgb(26, 26, 26);
}
.responsive-image {
  width: 100%;
  max-width: 800px;
  height: auto;
}
.cardContact {
  background-color: rgb(24, 24, 24);
  border-radius: 10px;
  padding: 20px;
  margin: 10px;
  text-align: center;
  color: white;
}
.cardContact i {
  margin-bottom: 15px;
}
.cardContact h1 {
  font-size: 1.5rem;
  margin: 10px 0;
}
.cardInstagram, .cardWhatsaap, .cardEmail {
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 5px;
  padding: 10px;
  margin: 5px 0;
}
.cardInstagram{
    margin: 0;
    color: rgb(255, 255, 255);
    border: 2px solid transparent;
    border-color: rgb(193, 53, 132);
    background-color: rgb(131, 58, 180, 0.356);
}
.cardWhatsaap{
    margin: 0;
    color: white;
    border: 2px solid transparent;
    border-color: rgb(37, 211, 102);
    background-color:rgb(7, 94, 84, 0.356);
}
.cardEmail{
    margin: 0;
    color: white;
    border: 2px solid transparent;
    border-color: rgb(0, 178, 255);
    background-color: rgba(0, 106, 255, 0.356);
}
</style>
