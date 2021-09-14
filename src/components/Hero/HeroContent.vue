<template>
    <div class="hero__content">
        <div class="hero__content__main">
            <h1>
                <span class="violet">A</span>YDEN<span class="pink">H</span>EX
            </h1>
            <h3>Software Engineer</h3>
            <button onclick="location.href='mailto:aydendevg@gmail.com';">Contact me!</button>
        </div>
        <img src="/src/assets/avatar.png" alt="avatar" />
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    h1 {
        font-size: 8em;
        font-weight: bolder;
        
    }

    h1, h3 {
        color: white;
        margin-top: 0;
        margin-bottom: 0;
    }

    h3 {
        font-size: 3em;
    }

    button {
        border: 2px var(--secondary-violet) solid;
        border-radius: 12px;
        background-color: var(--main-hero-bg);
        color: white;
        font-size: 1.5em;
        width: 10vw;
        padding: 0.4em;
        margin-top: 4rem;
    }

    button:hover {
        cursor: pointer;  
    }

    .hero__content {
        display: flex;
        justify-content: space-between;
        height: 75vh;
        width: 80vw;
        margin: auto;
        margin-top: 1rem;
    }

    .hero__content__main {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    .violet {
        color: var(--secondary-violet)
    }

    .pink {
        color: var(--secondary-pink)
    }
</style>