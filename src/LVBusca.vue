<template>
    <h3>Buscando rivais</h3>
    <label>Time:</label>
    <input type="text" v-model="busca">
    <p>Rival: {{ rival(busca) }}</p>
</template>

<script>
export default {
    name: 'LVBusca',
    data() {
        return {
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
