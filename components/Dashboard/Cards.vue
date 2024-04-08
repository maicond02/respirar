<template>
    <div class="flex w-12">
        <div class="col-3 shadow-2 border-round-sm card-temp">
            <p class="flex justify-content-center"><i class="pi pi-sun text-8xl"></i></p>
            <div class="flex flex-column align-items-center">
                <span class="text-4xl">28.6 C</span>
                <span class="text-xl">Clear sky</span>
            </div>
        </div>
        <div class="grid pt-0 pb-0 col-6 flex">
            <div class="pl-2 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Velocidade do vento</span>
                    <span class="text-2xl">28 km/h</span>
                </div>
            </div>
            <div class="pl-2 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Úmidade</span>
                    <span class="text-2xl">48%</span>
                </div>
            </div>
            <div class="pl-2 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Úmidade</span>
                    <span class="text-2xl">48%</span>
                </div>
            </div>
            <div class="pl-2 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Úmidade</span>
                    <span class="text-2xl">48%</span>
                </div>
            </div>
            <div class="pl-2 pb-0 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Úmidade</span>
                    <span class="text-2xl">48%</span>
                </div>
            </div>
            <div class="pl-2 pb-0 pr-2 col-6">
                <div class="shadow-2 card-temp border-round-sm flex flex-column align-items-center p-4">
                    <span>Úmidade</span>
                    <span class="text-2xl">48%</span>
                </div>
            </div>
        </div>
        <div class="col-3 shadow-2 card-temp border-round-sm">
        </div>
    </div>
</template>

<style scoped>
    .card-temp{
        background-color: #29282f;
    }
</style>