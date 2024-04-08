
<template>
    <div class="flex">
        <div class="w-2">
            <DashboardMenuLateral class="menu-lateral w-2"/>
        </div>
        <div class="w-10 p-4">
            <DashboardMenuTop />
            <DashboardCards class="mt-4"/>
            <DashboardTable class="mt-4"/>
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
