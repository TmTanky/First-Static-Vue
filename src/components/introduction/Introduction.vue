<template>
    <main>
        <div class="introleft">
            <h1> Hi welcome to my first <span class="vue" @click="redirectToVue">Vue</span>. </h1>
            <p> It's my <strong>8th</strong> month of journey of learning <strong>web development</strong> and I'm currently learning <strong>Vue JS</strong>. </p>
        </div>
    </main>
</template>

<script>
export default {
    methods: {
        redirectToVue() {
            window.open('https://vuejs.org/', '_blank')
        }
    }
}
</script>

<style scoped>

main {
    display: flex;
    justify-content: flex-start;
    padding: 13rem 2rem;
}

.vue {
    text-decoration: underline;
    color: #42b883;
}

.vue:hover {
    cursor: pointer;
}

h1 {
    font-size: 6vw;
}

p {
    margin-top: 1rem;
    font-size: 2vw;
}

@media screen and (max-width: 750px) {

    main {
        padding: 10rem 1rem;
    }

    .vue {
        font-size: 9vw;
    }

    h1 {
        font-size: 8vw;
    }

    p {
        font-size: 4vw;
    }

}

@media screen and (max-width: 500px) {

    main {
        padding: 10rem 1rem;
    }

    .vue {
        font-size: 9vw;
    }

    h1 {
        font-size: 10vw;
    }

    p {
        font-size: 6vw;
    }

}

</style>