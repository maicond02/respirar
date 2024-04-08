<template>
    <div class="flex justify-content-center mt-6">
        <img class="imagemLogo" src="/public/LOGORESP.png"/>
        <div class="cardForm col-4 ">
            <h1 class="m-4 flex justify-content-center align-content-start">Login</h1>
            <label class="m-4 flex justify-content-center align-content-start">Welcome to the Intelligent Air Purification System. Register or log in to experience.</label>
            <div class="formStyle flex flex-column gap-2 p-4">
                <label>E-mail</label>
                <InputText id="emailForm" v-model="value"/>
                <small id="email-help">Enter your E-mail aderess.</small>
            </div>
            <div class="flex flex-column gap-2 pr-4 pb-4 pl-4">
                <label>Password</label>
                <InputText id="emailForm" v-model="value"/>
                <small id="Password-help">Enter your Password.</small>
            </div>
            <div class="card flex justify-content-start p-4">
                <Checkbox v-model="Checkbox" :binary="true" />
                <label class="pl-2">I agree to terms of service</label>
            </div>
            <div class="card flex justify-content-center">
                <Button class="buttonLogin w-9 m-4" label="Submit" />
            </div>
        </div>
    </div>
</template>

<script>
    const checked = ref(false);
</script>

<style scoped>

.cardLogin{
    background-color: transparent;
    border-radius: 0%;
    height: 100%;
    width: 100%;
}
.cardForm{
    border-top-right-radius: 3% !important;
    border-top-left-radius: 0% !important;
    border-bottom-left-radius: 0% !important;
    border-bottom-right-radius: 3% !important;
    background-color: rgb(32, 32, 32);
}
.imagemLogo{
    width:50%;
    height: 50%;
    border-top-left-radius: 3%;
    border-bottom-left-radius: 3%;
}
.buttonLogin{

}

</style>