<template>
    <div>
        <h2>About</h2>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nam numquam consectetur quod qui necessitatibus alias, perferendis nisi cumque facilis aspernatur, corporis officia natus, unde minus accusantium sequi dignissimos distinctio culpa.</p>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nam numquam consectetur quod qui necessitatibus alias, perferendis nisi cumque facilis aspernatur, corporis officia natus, unde minus accusantium sequi dignissimos distinctio culpa.</p>
        <div>{{ data }}</div>
    </div>
</template>

<script setup>
// const {data} = await useFetch('/api/kukuh?name=mario', {
//     method: 'POST',
//     body: {
//         age: 20
//     }
// })

// const {data} = await useFetch('/api/kukuh')
const {data} = await useFetch('/api/currency/GBP')
</script>

<style lang="scss" scoped>
h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

p {
    margin: 20px 0;
}

</style>