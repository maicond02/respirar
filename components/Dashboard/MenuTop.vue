<template>
    <div class="flex">
        <div>
            <IconField iconPosition="left">
                <InputIcon class="pi pi-search"> </InputIcon>
                <InputText v-model="value1" placeholder="Search" />
            </IconField>
        </div>
        <div class="flex justify-content-end w-12 align-items-center">
            <Button icon="pi pi-cog" severity="secondary" text rounded aria-label="Notification" />
            <Button icon="pi pi-bell" severity="secondary" text rounded aria-label="Notification" />
            <Avatar icon="pi pi-user" class="ml-2 mr-2" shape="circle" />
        </div>
    </div>
</template>
<script>


</script>