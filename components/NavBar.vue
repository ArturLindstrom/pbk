<template>
<div>
    <nav>
        <ul>
            <li><nuxt-link to="/"><img class="nav-img" src="assets/pbk.svg"></nuxt-link></li>
            <li><nuxt-link to="/about">Om Powerballadkören</nuxt-link></li>
            <li><nuxt-link to="/contact">Kontakt</nuxt-link></li>
        </ul>
    </nav>
</div>
</template>

<script setup>

</script>

<style scoped lang='scss'>
  nav {
    display: flex;
    justify-content: center;
    height: 10vmin;
  }


  ul {
    appearance: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
    list-style: none;
  }

  .nav-img {
    height: 8vmin;
  }

  a {
    text-decoration: none;
    font-family: 'Josefin Sans', sans-serif;
    font-size: 2rem;
    color: #000;
    &:visited{
      color: #000;
    }
  }
  a.router-link-exact-active{
    color: #52BDA9;
    font-size: 2.5rem;
    
  
}
</style>