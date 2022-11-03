<template>
  <main>
    <a href="https://www.instagram.com/powerballadkoren/">
      <img class="img" src="/assets/pbk.svg" alt="Powerballadkoren" />
    </a>
  </main>
 
</template>
<script setup>

</script>

<style scoped lang='scss'>
main {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 75vh;
}
.img {
  width: 40vw;
  transition: all 0.25s ease;
}

.img:hover {
  filter: brightness(1.05);
  scale: 1.05;
  transition: all 0.5s ease;
}
 
</style>