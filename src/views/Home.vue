<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <div>
      {{ $t('my_name') }}
    </div>
    <HelloWorld :msg="$t('message')"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
