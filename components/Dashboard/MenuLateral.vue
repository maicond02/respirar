<template>
    <div class="card flex justify-content-start">
        <Menu :model="items" />
        <Dialog v-model:visible="visibleMessages" modal header="Mensagens">
            <DataTable :value="systemMessages" class="w-12">
                <Column field="id" header="ID"></Column>
                <Column field="message" header="Mensagem"></Column>
                <Column field="date" header="Data"></Column>
                <Column field="status" header="Status"></Column>
            </DataTable>
        </Dialog>
        <Dialog v-model:visible="visibleAdj" modal header="Ajustes">
            <TabView>
                <TabPanel header="Sensores">
                    <h3>Gerenciar Sensores</h3>
                    <DataTable :value="sensors" class="w-12">
                        <Column field="id" header="ID"></Column>
                        <Column field="nome" header="Nome"></Column>
                        <Column field="status" header="Status"></Column>
                        <Column header="Ações">
                            <template #body="slotProps">
                                <div>
                                    <i class="pi pi-pencil"></i>
                                </div>
                            </template>
                        </Column>
                    </DataTable>
                </TabPanel>
                <TabPanel header="Conta">
                    <h3>Configurações da Conta</h3>
                    <div class="p-fluid">
                        <div class="p-field">
                            <label for="username">Nome de Usuário</label>
                            <InputText id="username" v-model="user.username" />
                        </div>
                        <div class="p-field">
                            <label for="email">Email</label>
                            <InputText id="email" v-model="user.email" />
                        </div>
                        <div class="p-field">
                            <label for="password">Senha</label>
                            <Password id="password" v-model="user.password" toggleMask />
                        </div>
                        <Button label="Salvar" @click="visibleAdj = false"</Button>
                    </div>
                </TabPanel>
            </TabView>
        </Dialog>
    </div>
</template>

<script>
export default {
    data() {
        return {
            visibleMessages:false,
            visibleAdj:false,
            systemMessages: [
                { id: 1, message: 'Sistema iniciado com sucesso.', date: '01/01/2024', status: 'Info' },
                { id: 2, message: 'Erro ao conectar ao banco de dados.', date: '02/01/2024', status: 'Erro' },
                { id: 3, message: 'Atualização disponível.', date: '03/01/2024', status: 'Aviso' },
                { id: 4, message: 'Backup realizado com sucesso.', date: '04/01/2024', status: 'Sucesso' }
            ],
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
                            icon: 'pi pi-envelope',
                            command: () => {
                                this.visibleMessages = true;
                            }
                        },
                    ]
                },
                {
                    label: 'Profile',
                    items: [
                        {
                            label: 'Ajustes',
                            icon: 'pi pi-cog',
                            command: () => {
                                this.visibleAdj = true;
                            }
                        },
                        {
                            label: 'Sair',
                            icon: 'pi pi-sign-out',
                            command: () => {
                                this.$router.push('/');
                            }
                        }
                    ]
                }
            ],
            sensors: [
                { id: 1, nome: 'Sala de inglês', status: 'Ativo' },
                { id: 2, nome: 'Sala de matemática', status: 'Inativo' },
                { id: 3, nome: 'Sala de português', status: 'Ativo' }
            ],
            user: {
                username: 'Maicon_Admin',
                email: 'maicondouglas.md45@gmail.com',
                password: ''
            }
        };
    }
};
</script>
<style scoped>
    :deep(.p-menu){
        border: none !important;
    }
    .p-dialog .p-dialog-content {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .p-field {
        width: 100%;
        margin-bottom: 1em;
    }

    .p-field label {
        font-weight: bold;
    }

    .p-field input {
        width: 100%;
    }

</style>
