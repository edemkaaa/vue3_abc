<script>
export default {
    props: ['name', 'surn', 'age'],
    data() {
	return {
		newName: '',
		newSurn: '',
	}
}
}
</script>

<template>
	{{ name }}
	{{ surn }}
	{{ age }}
</template>