<template>
    <div class="grid flex justify-content-center">
        <h1 class="Titulo">
        Let's Talk
        </h1>
    </div>
    <div class="grid flex justify-content-center">
        <div class="card flex flex-column justify-content-center col-12 md:col-4" >
            <label class="pt-3 px-0" for="FullName">FullName</label>
            <InputText class="" id="username" v-model="fullName" aria-describedby="username-help" />
            <small>Enter your full name.</small>
            <label class="pt-5 px-0-3" for="Email">E-mail</label>
            <InputText class="" id="email" v-model="email" aria-describedby="email-help" />
            <small>Enter your E-mail.</small>
            <label class="pt-5 px-0-3" for="Message">Message</label>
            <div class="pt-3 px-0-3" id="editor" contenteditable>
              Type here.
            </div>
            <small>Enter your message.</small>
        </div>
    </div>
    <div class="flex justify-content-center">
        <img class="col-6" src="/public/Contac.png">
    </div>

    <Divider align="center" type="dotted">
        <b>Other media</b>
    </Divider>
  <div class="grid col-12 flex justify-content-center align-content-center">
      <div class="cardContact col-12 sm:col-3 mt-7 mb-5 mr-5 ml-5">
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

      <div class="cardContact col-12 sm:col-3 mt-5 mb-0 mr-5 ml-5">
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

      <div class="cardContact col-12 sm:col-3 mt-7 mb-5 mr-5 ml-5">
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

<style #scoped>
.Titulo {
  font-size: 5rem;
}
.card {
  background-color: rgb(32, 32, 32);
  border-radius: 7px;
}
#editor {
border: 1px solid rgb(32, 32, 32);
background-color: rgb(9, 9, 11);
min-height: 200px;
overflow: auto;
}
.responsive-image {
    width: 100%;
    max-width: 800px;
    height: auto;
}

</style>