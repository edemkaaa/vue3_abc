<script>
export default {
    props: {
        id: Number,
        name: String,
        surn: String,
    },
    emits: ['change'],
    data() {
        return {
            isEdit: false,
            newName: this.name,
            newSurn: this.surn,
        }
    },
    methods: {
        edit(){
            this.isEdit = true;
        },
        save(){
            this.isEdit = false;
            this.$emit('change', this.id, this.newName, this.newSurn);
        }
    }
}
</script>

<template>
    <template v-if="!isEdit">
    <p class="employee">{{ name }} {{ surn }}</p>
    <button class="button" @click="edit">edit</button>
</template>
    <template v-else>
        <input class="text-field__input" v-model="newName">
        <input class="text-field__input" v-model="newSurn">
        <button class="button" @click="save">save</button>
    </template>
</template>