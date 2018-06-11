<template>
  <div>
    <ul>
      <li><a :href="link_1.link_1_href" target="_blank">{{link_1.link_1_text}}</a></li>
      <li><a :href="link_2.link_2_href" target="_blank">{{link_2.link_2_text}}</a></li>
      <li><a :href="link_3.link_3_href" target="_blank">{{link_3.link_3_text}}</a></li>
      <li><a :href="link_4.link_4_href" target="_blank">{{link_4.link_4_text}}</a></li>
    </ul>
  </div>
</template>

<script>
import list from './list.vue'
export default {
    props : ["listElem"]
}
</script>

<style>
h1, h2 {
  font-weight: normal;
}
</style>
