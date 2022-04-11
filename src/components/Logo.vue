<template>
  <div id="logo">
    <img :src="logo"/>
  </div>
</template>

<script>
import SVG from "@/assets/cryptofactory_logo-01.svg"

export default {
  name: 'Logo',
  data () {
    return {
      logo: SVG
    }
  }
}
</script>

<style scoped>
#logo {
  position: absolute;
  left: 120px;
  display: block;
  width: 153px;
  height: 196px;
}

</style>