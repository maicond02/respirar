<template>
    <div class="flex w-12">
        <div class="col-3 shadow-2 border-round-sm card-temp">
            <p class="flex justify-content-center"><i class="pi pi-sun text-8xl"></i></p>
            <div class="flex flex-column align-items-center">
                <span class="text-4xl">19.6 C</span>
                <span class="text-xl">Clear sky</span>
                <Divider />
                <span class="text-xl">Americana - SP</span>
                <span class="text-xl">04 de junho de 2024</span>
            </div>
        </div>
        <div class="grid pt-0 pb-0 col-6 flex">
            <div class="pl-2 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex justify-content-center align-items-center p-4">
                    <div>
                        <i class="pi pi-flag text-4xl mr-4" />
                    </div>
                    <div class="flex flex-column">
                        <span>Velocidade do vento</span>
                        <span class="text-2xl">23 km/h</span>
                    </div>
                </div>
            </div>
            <div class="pl-2 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex justify-content-center align-items-center p-4">
                    <div>
                        <i class="pi pi-gauge text-4xl mr-4" />
                    </div>
                    <div class="flex flex-column">
                        <span>Úmidade</span>
                        <span class="text-2xl">54%</span>
                    </div>
                </div>
            </div>
            <div class="pl-2 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex justify-content-center align-items-center p-4">
                    <div>
                        <i class="pi pi-gauge text-4xl mr-4" />
                    </div>
                    <div class="flex flex-column">
                        <span>Pressão</span>
                    <span class="text-2xl">1021 mb</span>
                    </div>
                </div>
            </div>
            <div class="pl-2 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Visibilidade</span>
                    <span class="text-2xl">12,87km</span>
                </div>
            </div>
            <div class="pl-2 pb-0 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Nascer do sol</span>
                    <span class="text-2xl">06:43</span>
                </div>
            </div>
            <div class="pl-2 pb-0 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Por do sol</span>
                    <span class="text-2xl">17:31</span>
                </div>
            </div>
        </div>
        <div class="col-3 shadow-2 card-temp border-round-sm">
            <div class="flex flex-column align-items-center">
                <span class="text-4xl mb-4">Sensores conectados</span>
                <span class="text-xl mb-4">Sala de inglês</span>
                <span class="text-xl mb-4">Sala de matemática</span>
                <span class="text-xl mb-4">Sala de português</span>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .card-temp{
        background-color: #29282f;
    }
</style>