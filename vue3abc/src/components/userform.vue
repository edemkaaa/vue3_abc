<script>
export default {
    data() {
        return {
            newName: ' ',
            newSurn: ' ',
        }
    },
    methods: {
        save(){
            this.$emit('add', this.newName, this.newSurn)
        }
    }
}
</script>

<template>
    <input class="header" v-model="newName">
    <br>
    <br>
    <input class="header" v-model="newSurn">
    <br>
    <button class="logo" @click="save">save</button>
</template>