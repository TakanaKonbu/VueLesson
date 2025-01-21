<script>

import {defineComponent} from "vue";
import TopImage from "@/components/topimage.vue";
import Content from "@/components/content.vue";
import SideMenu from "@/components/sidemenu.vue";

export default defineComponent({
  components: {SideMenu, Content, TopImage},
  data() {
    return {
      premiumContent:{
        imageSrc: "/img/premium.jpg",
        textItems: ["Sample Text 1", "Sample Text 2", "Sample Text 3"]
      },

      standardContent: {
        imageSrc: "/img/standard.jpg",
        textItems: ["Test Text 1", "Test Text 2", "Test Text 3"]
      }
    }
  }
})
</script>

<template>
  <TopImage />
  <div class="main-container">
    <div class="content-area">
      <Content
          :imageSrc="premiumContent.imageSrc"
          :textItems="premiumContent.textItems"
      />
      <Content
          :imageSrc="standardContent.imageSrc"
          :textItems="standardContent.textItems"
      />
    </div>
    <SideMenu class="side-menu" />
  </div>
</template>

<style scoped>
.main-container {
  display: flex;
  gap: 2rem;
  margin-top: 2rem;
}

.content-area {
  flex: 3;  /* コンテンツエリアを3の比率で */
}

.side-menu {
  flex: 1;  /* サイドメニューを1の比率で */
}
</style>