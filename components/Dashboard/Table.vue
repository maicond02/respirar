<template>
    <div class="grid flex w-12 mt-4">
        <DataTable :value="values" class="w-12">
            <Column field="id" header="Code"></Column>
            <Column field="leitura" header="Leitura"></Column>
            <Column field="data" header="Data de Leitura"></Column>
            <Column field="valor" header="Valor"></Column>
            <Column header="Info">
                <template #body="slotProps">
                    <div>
                        <i class="pi pi-info-circle" @click="showDetails()"></i>
                    </div>
                </template>
            </Column>
        </DataTable>
    </div>
    <Dialog v-model:visible="visible" modal header="Dados de poluentes">
        <DataTable :value="pollutantData" class="w-12">
            <Column field="pollutant" header="Poluentes"></Column>
            <Column field="mp10" header="MP10"></Column>
            <Column field="mp25" header="MP2.5"></Column>
            <Column field="nox" header="NOx"></Column>
            <Column field="o3" header="O3"></Column>
            <Column field="sox" header="SOx"></Column>
            <Column field="co" header="CO"></Column>
            <Column field="pts" header="PTS"></Column>
            <Column field="fumaca" header="Fumaça"></Column>
            <Column field="cn" header="CN"></Column>
        </DataTable>
    </Dialog>
</template>

<script>

export default {
    data() {
        return {
            values: [
                {id: 1, leitura: 'Média qualidade do ar', data: '01/01/2024', valor: '70%'},
                {id: 2, leitura: 'Baixa qualidade do ar', data: '02/01/2024', valor: '40%'},
                {id: 3, leitura: 'Boa qualidade do ar', data: '03/01/2024', valor: '100%'},
                {id: 4, leitura: 'Boa qualidade do ar', data: '04/01/2024', valor: '100%'},
                {id: 5, leitura: 'Boa qualidade do ar', data: '05/01/2024', valor: '100%'},
                {id: 6, leitura: 'Baixa qualidade do ar', data: '06/01/2024', valor: '40%'},
                {id: 7, leitura: 'Boa qualidade do ar', data: '07/01/2024', valor: '100%'},
                {id: 8, leitura: 'Boa qualidade do ar', data: '08/01/2024', valor: '100%'},
                {id: 9, leitura: 'Boa qualidade do ar', data: '09/01/2024', valor: '100%'},
                {id: 10, leitura: 'Boa qualidade do ar', data: '10/01/2024', valor: '100%'},
                {id: 11, leitura: 'Boa qualidade do ar', data: '11/01/2024', valor: '100%'},
                {id: 12, leitura: 'Média qualidade do ar', data: '12/01/2024', valor: '70%'},
                {id: 13, leitura: 'Boa qualidade do ar', data: '13/01/2024', valor: '100%'},
                {id: 14, leitura: 'Baixa qualidade do ar', data: '14/01/2024', valor: '40%'},
                {id: 15, leitura: 'Boa qualidade do ar', data: '15/01/2024', valor: '100%'},
                {id: 16, leitura: 'Boa qualidade do ar', data: '16/01/2024', valor: '100%'},
                {id: 17, leitura: 'Baixa qualidade do ar', data: '17/01/2024', valor: '40%'},
                {id: 18, leitura: 'Média qualidade do ar', data: '18/01/2024', valor: '70%'},
                {id: 19, leitura: 'Baixa qualidade do ar', data: '19/01/2024', valor: '40%'},
                {id: 20, leitura: 'Média qualidade do ar', data: '20/01/2024', valor: '70%'}
            ],
            pollutantData: [
                { pollutant: 'Nº total', mp10: 233, mp25: 96, nox: 140, o3: 137, sox: 98, co: 96, pts: 109, fumaca: 10, cn: 4 },
                { pollutant: '%', mp10: 62.8, mp25: 25.9, nox: 37.7, o3: 36.9, sox: 26.4, co: 25.9, pts: 29.4, fumaca: 2.7, cn: 1.1 }
            ],
            visible:false

        };
    },
    methods:{
        showDetails(){
            this.visible = true;
        }
    },
    mounted() {
        //ProductService.getProductsMini().then((data) => (this.products = data));
    }
};
</script>