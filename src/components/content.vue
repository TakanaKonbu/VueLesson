<script>
export default {
  name: 'Content'
}
</script>

<template>
  <div class="content">
    <div class="image-container">
      <img src="/img/premium.jpg" alt="Premium Image">
    </div>
    <div class="shoeText">
      <ul>
        <li>Sample Text 1</li>
        <li>Sample Text 2</li>
        <li>Sample Text 3</li>
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
