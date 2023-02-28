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
	save() {
		this.$emit('add', this.newName, this.newSurn);
	}
}
}
</script>

<template>
	<input v-model="newName">
	<input v-model="newSurn">
	
	<button @click="save">
		save
	</button>
</template>