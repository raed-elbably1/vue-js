<template>
  <div class="home">
    <HelloWorld />
    <ToodsList/>
    <React/>
   <Apphelp/>
   <Toods/>
   <comuniction/>
   <infosection/>
  </div>
</template>

<script>
import Apphelp from '@/components/Apphelp.vue';
import Comuniction from '@/components/comuniction.vue';
import HelloWorld from '@/components/HelloWorld.vue';
import Infosection from '@/components/infosection.vue';
import React from '@/components/React.vue';
import Toods from '@/components/Toods.vue';
import ToodsList from '@/components/ToodsList.vue';


export default {
  name: 'HomeView',
  components: {
       HelloWorld,
       ToodsList,
      React,
      Apphelp,
      Toods,
      Comuniction,
      Infosection
    }
}
</script>
