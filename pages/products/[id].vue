<template>
    <div>
        <p>Product details for {{ id }}</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae ipsam, repudiandae perspiciatis nemo ipsa dignissimos enim cum cumque minima facere quas eveniet porro alias similique non eos eum facilis odit.</p>
    </div>
</template>

<script setup>
const {id} = useRoute().params
</script>

<style scoped>

</style>