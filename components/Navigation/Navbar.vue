
<template>
    <nav class="card">
        <Menubar :model="items" >
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
                    label: 'Home',
                    icon: 'pi pi-home'
                },
                {
                    label: 'About',
                    icon: 'pi pi-book'
                },
                {
                    label: 'Contact',
                    icon: 'pi pi-envelope'
                },
                {
                    label: 'Buy',
                    icon: 'pi pi-dollar'
                }
            ]
        };
    }
};
</script>
