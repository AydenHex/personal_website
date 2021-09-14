<template>
    <div class="navbar">
        <a href="https://github.com/AydenHex" target="_blank">Github</a>
        <a href="https://dev.to/aydenhex" target="_blank">Dev.to</a>
        <a href="https://www.twitch.tv/ayden_hex" target="_blank">Twitch</a>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
a {
    color: white;
    font-size: 2.5em;
    font-weight: bolder;
    text-decoration: none;
}

a:hover {
    /* border-bottom: 2px var(--secondary-pink) solid; */
    text-decoration: underline;
    text-decoration-color: var(--secondary-pink);
}

.navbar {
    width: 90%;
    display: flex;
    justify-content: flex-end;
    gap: 4vw;
    padding-top: 4vh;
    padding-right: 4vh;
}
</style>