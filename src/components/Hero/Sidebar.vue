<template>
  <div class="hero__sidebar">
      <a href="https://www.linkedin.com/in/quentinroyer-25/" target="_blank"><img src="/src/assets/socials/linked-in.svg" alt="linkedin" /></a>
      <a href="https://twitter.com/DevAyden/" target="_blank"><img src="/src/assets/socials/twitter.svg" alt="twitter" /></a>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    @media (max-device-width: 480px ) {
        .hero__sidebar {
            position: absolute;
            width: 100%;
            display: flex;
            gap: 1rem;
            bottom: 8vh;
            justify-content: center;
        }
        a {
            text-decoration: none;
            padding: 1rem;
        }
        img {
            width: 3rem;
            height: auto;
            filter: invert(66%) sepia(7%) saturate(2670%) hue-rotate(202deg) brightness(92%) contrast(90%);
        }
    }
    @media (min-device-width: 481px ) {
        .hero__sidebar {
            position: absolute;
            width: 10rem;
            display: flex;
            bottom: 15vh;
            flex-direction: column-reverse;
            gap: 1rem;
        }
        a {
            text-decoration: none;
            padding: 1rem;
        }
        img {
            width: 5rem;
            height: auto;
            filter: invert(66%) sepia(7%) saturate(2670%) hue-rotate(202deg) brightness(92%) contrast(90%);
        }
    }
   
</style>