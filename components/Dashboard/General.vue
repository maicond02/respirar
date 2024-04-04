
<template>
    <div class="flex">
        <div class="w-2">
            <div class="menu-lateral w-2 flex justify-content-start">
                <DashboardMenuLateral />
            </div>
        </div>
        <div class="w-10">
            <DashboardMenuTop />
        </div>
    </div>
</template>

<style scoped>
.menu-lateral {
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0; 
    background-color: #18181b;
    border-radius: 10px;
    border-right: 1px rgb(58, 58, 58) solid;
}
</style>
