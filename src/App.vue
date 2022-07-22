<script>
import Navbar from '@/components/Navbar.vue';
import Section from '@/components/Section.vue';
import TitleAndSub from '@/components/TitleAndSub.vue';
import Works from '@/components/a.vue';

export default {
  components: {
    Navbar,
    Section,
    TitleAndSub,
    Works,
  }
}
</script>

<template>
  <Navbar/>
  <div class="columns">
      <TitleAndSub title="HOLA" subtitle="a" />
      <Section/>
  </div>
    <div class="columns">
      <Section/>
      <TitleAndSub title="Hola2" subtitle="b"/>
    </div>
    <Works/>

</template>