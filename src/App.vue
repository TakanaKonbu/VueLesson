<script>

import {defineComponent} from "vue";
import TopImage from "@/components/topimage.vue";
import Content from "@/components/content.vue";

export default defineComponent({
  components: {Content, TopImage}
})
</script>

<template>
  <TopImage />
  <Content />
</template>

<style scoped>

</style>
