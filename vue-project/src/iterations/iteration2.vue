<script>
export default {
    data() {
        return {
            sumOperationA: 5 + 5
        }
    },
    methods: {
        sumItems(a, b) {
            return a + b
        }
    },
    mounted() {
        this.$el.textContent += 'aaaa'
    }
}
</script>

<template>
    <div class="operation">
        <p>Sum 1: {{ 5 + 5 }} / </p>
        <p>Sum 2: {{ sumOperationA }} / </p>
        <p>Sum 3: {{ sumItems(5, 5) }} / </p>
    </div>
</template>

<style>
.operation {
    display: flex;
    justify-content: center;
    border: 1.5px solid rgb(0, 0, 0);
    margin-bottom: 40px;
}
</style>