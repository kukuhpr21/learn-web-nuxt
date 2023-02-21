<template>
    <div>
        <header>
            <nav>
                <nuxt-link to="/">Nuxt Kukuh</nuxt-link>
                <ul>
                    <li><nuxt-link to="/">Home</nuxt-link></li>
                    <li><nuxt-link to="/about">About</nuxt-link></li>
                    <li><nuxt-link to="/products">Products</nuxt-link></li>
                </ul>
            </nav>
        </header>
        <div>
            <slot/>
        </div>
    </div>
</template>

<style scope>
.router-link-exact-active {
    color: #12b488;
}
</style>