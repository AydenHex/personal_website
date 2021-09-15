<template>
    <div class="mobile__navbar">
        <Slide right>
            <div class="navbar">
                <a href="https://github.com/AydenHex" class="test" target="_blank">Github</a>
                <a href="https://dev.to/aydenhex" target="_blank">Dev.to</a>
                <a href="https://www.twitch.tv/ayden_hex" target="_blank">Twitch</a>
            </div>
        </Slide> 
    </div>
    <div class="desktop__navbar">
        <div class="navbar">
            <a href="https://github.com/AydenHex" class="test" target="_blank">Github</a>
            <a href="https://dev.to/aydenhex" target="_blank">Dev.to</a>
            <a href="https://www.twitch.tv/ayden_hex" target="_blank">Twitch</a>
        </div>
    </div>
</template>

<script>
import { Slide } from 'vue3-burger-menu'
import Sidebar from '../Sidebar.vue'
export default {
    components: {Slide}
}
</script>

<style scoped>

a {
    color: white;
    text-decoration: none;
    font-weight: bolder;
}
@media (max-device-width : 480px) {

    .desktop__navbar {
        display: none;
    }
    :deep() .bm-burger-button {
        left: 80vw;
    }

    :deep() .bm-menu {
        background-color: var(--secondary-violet);
    }

    a {
        font-size: 2.5em;
    }

    .navbar {
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin-right: 2rem;
        gap: 6vw;
        text-align: center;
    }

    .mobile__navbar {
        display: flex;
        flex-direction: column;
    }

}


@media (min-device-width : 481px) {
    :deep() .bm-burger-button {
        display: none;
    }
    a {
        font-size: 2.5em;
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
}

</style>