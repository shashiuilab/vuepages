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
export default {
data () {
    return {
        link_1 : {
            link_1_href:"https://vuejs.org",
            link_1_text : "Core Docs"
        },
        link_2 :  {
            link_2_href:"https://forum.vuejs.org",
            link_2_text : "Forum"
        },
        link_3  : {
            link_3_href:"https://chat.vuejs.org",
            link_3_text : "Community Chat"
        },
        link_4  : {
            link_4_href:"https://twitter.com/vuejs",
            link_4_text : "Twitter"
        }
    }
    },
    beforeCreate : function() {
        console.log("Before create");
    },
    created : function() {
        console.log("created");
    },
    beforeUpdate : function() {
        console.log("Before update");
    },
    updated : function() {
        console.log("updated");
    },
    beforeMount : function() {
        console.log("Before mount");
    },
    mounted : function() {
        console.log("Mounted");
    }
}
</script>

<style>
h1, h2 {
  font-weight: normal;
}
</style>
