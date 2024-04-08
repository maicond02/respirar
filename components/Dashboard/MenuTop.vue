<template>
    <div class="flex">
        <div>
            <IconField iconPosition="left">
                <InputIcon class="pi pi-search"> </InputIcon>
                <InputText v-model="value1" placeholder="Search" />
            </IconField>
        </div>
        <div class="flex justify-content-end w-12 align-items-center">
            <Dropdown v-model="selectedAparelho" :options="aparelhos" optionLabel="name" placeholder="Selecione" class="w-full md:w-14rem" />
            <Button icon="pi pi-cog" severity="secondary" text rounded aria-label="Notification" />
            <Button icon="pi pi-bell" severity="secondary" text rounded aria-label="Notification" />
            <Avatar icon="pi pi-user" class="ml-2 mr-2" shape="circle" />
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            selectedAparelho: null,
            aparelhos: [
                { name: 'Sala Inglês', code: '0' },
                { name: 'Sala Matemática', code: '1' },
                { name: 'Sala Português', code: '2' },
            ]
        };
    }
};
</script>