<template>
  <nuxt-link :to=props.link>
    <div class="nav-ball" :class="{'is-active': isActive, 'img': img}">
          <slot />
      </div>
  </nuxt-link>
</template>

<script setup>
const props = defineProps({
  link: {
    type: String,
    required: true
  },
  img: {
    type: Boolean,
    default: false
  }
})

const route = useRoute()
const currentPath = computed(() => route.path)

const isActive = computed(() => {
  return currentPath.value === props.link
})

const img = computed(() => {
  return props.img
})

const ballClass = computed(() =>{
  if (isActive.value) {
    return 'is-active'
  } else if (img.value) {
    return 'image'
  }
})


</script>

<style scoped lang='scss'>
  .nav-ball {
    display: grid;
    place-items: center;
    align-items: center;
    height: 5rem;
    width: 5rem;
    border-radius: 50%;
    background-color: #52bda95c;
    transition: all 0.3s ease-in-out;
  }
  .nav-ball:hover {
    background-color: #52bda9;
    transition: all 0.3s ease-in-out;
  }

  a {
  text-decoration: none;
  font-family: 'Josefin Sans', sans-serif;
  color: #d98ab7;
  font-size: 1.2rem;
    &:visited {
    color: #d98ab7;
    }
  }
  .is-active {
    background-color: #52bda9;
    color: #fff;
}
  .img {
    height: 7.5rem;
    width: 7.5rem;
  }


</style>