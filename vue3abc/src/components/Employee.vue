<script>
export default {
    props: ['name'],
    data() {
        return {
        }
    }
}
</script>

<template>
<ul class="styled">
    <li v-for="user in name">{{ user }}</li>
</ul>
</template>