
<template>
    <nav class="card">
        <Menubar :model="items" class="">
            <template #end>
                <div class="flex align-items-center gap-2">
                    <Button @click="$router.push('/user/login')" class="hidden md:block" label="Login" severity="secondary" text raised />
                    <Button @click="$router.push('/user/register')"  class="hidden md:block" label="Register"/>
                    <InputText class="hidden md:block" type="text"/>
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
                    label: 'INÍCIO',
                    icon: 'pi pi-home',
                    command: () => {
                        this.$router.push('/');                    
                    }
                },
                {
                    label: 'SOBRE',
                    icon: 'pi pi-book',
                    command: () => {
                        this.$router.push('/about');                    
                    }
                },
                {
                    label: 'CONTATO',
                    icon: 'pi pi-envelope',
                    command: () => {
                        this.$router.push('/contact');                    
                    }
                },
                {
                    label: 'INSTALAÇÃO',
                    icon: 'pi pi-dollar',
                    command: () => {
                        this.$router.push('/buy');                    
                    }                
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

</style>
