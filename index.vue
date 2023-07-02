<template>
    <div>
        <h1>{{ message }}</h1>
        <input v-model="inputText" type="text">
        <button @click="changeMessage">Ubah Pesan</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            message: 'Halo, dunia!',
            inputText: ''
        };
    },
    methods: {
        changeMessage() {
            this.message = this.inputText;
            this.inputText = '';
        }
    }
};
</script>

<style>
h1 {
    color: blue;
}
</style>
