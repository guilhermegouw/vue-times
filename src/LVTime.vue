<template>
    <div>
        <h3>Buscando rivais</h3>
        <label>Time:</label>
        <input type="text" v-model="busca">
        <p>Rival: {{ rival(busca) }}</p>

        <h3>Perfil</h3>
        <p>Time: {{ nome }}</p>
        <p>Estádio: {{ estadio }}</p>
    </div>
</template>

<script>
export default {
    name: 'LVTime',
    data() {
        return {
            nome: 'Cruzeiro',
            estadio: 'Mineirão',
            busca: '',
        }
    },
    methods: {
        rival(time) {
            switch (time.toLowerCase()){

                case 'cruzeiro':
                    return 'atlético';
                case 'atlético':
                    return 'cruzeiro';
                case 'palmeiras':
                    return 'corinthians';
                case 'corinthians':
                    return 'palmeiras';
                case 'flamengo':
                    return 'vasco';
                default:
                    return 'não encontrado';
            }
        }
    }
}
</script>

<style>
</style>
