
<template>
    <nav class="card">
        <Menubar :model="items" class="">
            <template #end>
                <div class="flex align-items-center gap-2">
                    <Button label="Login" severity="secondary" text raised />
                    <Button label="Register"/>
                    <InputText type="text"/>
                </div>
            </template>
        </Menubar>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            items: [
                {
                    label: 'HOME',
                    icon: 'pi pi-home'
                },
                {
                    label: 'ABOUT',
                    icon: 'pi pi-book'
                },
                {
                    label: 'CONTACT',
                    icon: 'pi pi-envelope'
                },
                {
                    label: 'BUY',
                    icon: 'pi pi-dollar'
                }
            ]
        };
    }
};
</script>

<style scoped>
    :deep(.p-menubar){
        border: none;
    }
    :deep(.p-menuitem-text){

    }
    :deep(.p-menuitem-icon){

    }

</style>
