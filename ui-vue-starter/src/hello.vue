<template>
    <form style="width: 300px;">
        <sp-heading>
            {{ message }}
        </sp-heading>
        <sp-body>
            Button has been clicked {{ count }} times.
        </sp-body>
        <footer>
            <sp-button v-on:click="increment">Click me</sp-button>
        </footer>
    </form>
</template>

<script>
    module.exports = {
        methods: {
            increment() {
                this.count++;
            }
        },
        data() {
            return {
                reactive: true,
                message: 'Hello World Vue Component!',
                count: 0
            }
        }
    }
</script>
