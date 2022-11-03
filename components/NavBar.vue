<template>
    <nav>
        <div class="nav-items">
          <nav-ball link='/about'>Om oss</nav-ball>
          <nav-ball :img=true link='/'><img src="assets/pbk.svg" class="nav-img"></nav-ball>
          <nav-ball link='/contact'>Kontakt</nav-ball>
        </div>
    </nav>
</template>

<script setup>

</script>

<style scoped lang='scss'>
  nav {
    display: flex;
    justify-content: center;
    height: 25vh;
    background: none;
  }


  .nav-items {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    place-items: center;
    width: 100%;
  }

  .nav-img {
    width: 5rem;
    transform: translateY(0.5rem)
  }

</style>