<template>
    <main>
        <div class="contact1">
            <h2> Contact Me </h2>
        </div>

        <div class="contact2">
            <div class="item" @click="toGithub" > <img src="https://img.icons8.com/material-outlined/50/000000/github.png"/> </div>
            <div class="item" @click="toTwitter" > <img src="https://img.icons8.com/material-rounded/50/000000/twitter-squared.png"/> </div>
            <div class="item" @click="toFb" > <img src="https://img.icons8.com/material-outlined/50/000000/facebook-f.png"/> </div>
        </div>
    </main>
</template>

<script>
export default {
    methods: {
        toFb() {
            window.open('https://www.facebook.com/', '_blank')
        },
        toTwitter() {
            window.open('https://twitter.com/', '_blank')
        },
        toGithub() {
            window.open('https://github.com/TmTanky', '_blank')
        }
    }
}
</script>

<style scoped>

main {
    display: flex;
    padding: 5rem 2rem;
}

.contact1, .contact2 {
    flex: 1;
}

.contact1 h2 {
    font-size: 2rem;
    color: #42b883;
}

.contact2 {
    display: flex;
    justify-content: center;
}

.contact2 .item {
    margin: 0rem 1rem;
}

.item {
    cursor: pointer;
}

@media screen and (max-width: 500px) {
    
    main {
        flex-direction: column;
        padding: 3rem 1rem;
    }

    .contact1 {
        display: flex;
        justify-content: center;
        padding: 3rem 0rem;
    }

}

</style>