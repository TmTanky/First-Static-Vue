<template>
    <nav>
        <div class="navlogo">
            <h1> {{ hello }} </h1>
        </div>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            hello: "First Vue"
        }
    }
}
</script>

<style scoped>

nav {
    display: flex;
    justify-content: flex-start;
    background-color: #42b883;
    padding: 1rem 2rem;
}

.navlogo {
    color: white;
}

</style>