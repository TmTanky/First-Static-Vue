<template>
    <footer>
        <p> Copyright &copy; First Vue {{ year }}  </p>
    </footer>
</template>

<script>

const yearNow = new Date().getFullYear()

export default {
    data() {
        return {
            year: yearNow
        }
    }
}
</script>

<style scoped>

footer {
    display: flex;
    justify-content: center;
    background-color: #42b883;
    padding: 0.8em 0rem;
}

footer p {
    color: white;
}

</style>