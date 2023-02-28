<script>
export default {
    emits: ['show', 'show1'],
    data() {
        return {
        }
    },
    methods: {
        handleName() {
            this.$emit('show', 'Edem');
        },
        handleSalary(){
            this.$emit('show1', 'Elvin', '1200000');
        }
    }
}
</script>

<template>
<button class="button" @click="handleName">Name</button>
<button class="button" @click="handleSalary">Salary</button>
</template>