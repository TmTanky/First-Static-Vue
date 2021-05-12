<template>
    <main>
        <div class="item" v-for="item in myThoughts" :key="item.id" >
            <h3> {{ item.title }} </h3>
            <p> {{ item.content }} </p>
        </div>
    </main>
</template>

<script>
export default {
    data() {
        return {
            myThoughts: [
                {
                    id: 1,
                    title: "It's easy to use",
                    content: "For me it's very easy to use and easy to catch up."
                },
                {
                    id: 2,
                    title: "Beginner friendly",
                    content: "Beginner friendly for who wants to jump to frameworks."
                },
                {
                    id: 3,
                    title: "Easy syntax",
                    content: "Easy to remember syntax and to catch fundamentals."
                }
            ]
        }
    }
}
</script>

<style scoped>

main {
    display: flex;
    justify-content: space-evenly;
    padding: 7rem 2rem;
}

.item {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border-radius: 5px;
    padding: 1rem 2rem;
    text-align: center;
}

.item h3 {
    margin-bottom: 1rem;
    font-size: 1.5rem;
    text-transform: uppercase;
    color: #42b883;
}

@media screen and (max-width: 850px) {
    
    main {
        flex-direction: column;
        padding: 1rem 1rem;
    }
    
    .item {
        padding: 1rem;
    }

}

@media screen and (max-width: 500px) {
    
    .item {
        margin: 2rem 0rem;
    }

}

</style>