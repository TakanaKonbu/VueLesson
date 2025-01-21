<script>
export default {
  name: 'Content',
  // propsで外部からデータを受け取れるようにする
  props: {
    // 画像のパス
    imageSrc: {
      type: String,
      required: true
    },
    // テキストの配列
    textItems: {
      type: Array,
      required: true
    }
  }
}
</script>

<template>
  <div class="content">
    <div class="image-container">
      <!-- propsで受け取った画像パスを使用 -->
      <img :src="imageSrc" alt="">
    </div>
    <div class="shoeText">
      <ul>
        <!-- propsで受け取ったテキスト配列をループで表示 -->
        <li v-for="(text, index) in textItems" :key="index">{{ text }}</li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
  .content {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    gap: 20px;
  }

  .image-container {
    flex: 1;
    max-width: 50%;
  }

  .shoeText {
    flex: 1;
    max-width: 50%;
  }

  img {
    width: 100%;
    height: auto;
  }

  ul {
    list-style: none;
    padding: 0;
  }

  li {
    margin-bottom: 10px;
  }
</style>
