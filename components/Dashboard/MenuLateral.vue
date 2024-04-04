<template>
    <div class="card flex justify-content-center">
        <Menu :model="items" />
    </div>
</template>

<script>
export default {
    data() {
        return {
            items: [
                {
                    label: 'Navigation',
                    items: [
                        {
                            label: 'Início',
                            icon: 'pi pi-home',
                            command: () => {
                                this.$router.push('/user/dashboard');
                            }
                        },
                        {
                            label: 'Estatísticas',
                            icon: 'pi pi-chart-bar'
                        },
                        {
                            label: 'Mensagens',
                            icon: 'pi pi-envelope'
                        },
                    ]
                },
                {
                    label: 'Profile',
                    items: [
                        {
                            label: 'Ajustes',
                            icon: 'pi pi-cog'
                        },
                        {
                            label: 'Sair',
                            icon: 'pi pi-sign-out'
                        }
                    ]
                }
            ]
        };
    }
};
</script>
<style scoped>
    :deep(.p-menu){
        border: none !important;
    }
</style>
