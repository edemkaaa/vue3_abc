<script>
export default {
    props: ['name', 'surn', 'age'],
    data() {
        return {
        }
    }
}
</script>

<template>
   <p class="hunter">{{ name }}</p>
   <p class="hunter">{{ surn }}</p>
   <p class="hunter">{{ age }}</p>
</template>