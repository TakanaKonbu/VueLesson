<script>
  export default {
    name: 'SideMenu'
  }
</script>

<template>
  <div class="menuItem">
    <ul>
      <li>Menu 1</li>
      <li>Menu 2</li>
      <li>Menu 3</li>
      <li>Menu 4</li>
      <li>Menu 5</li>
    </ul>
  </div>
</template>

<style scoped>
  .menuItem {
    background-color: #f5f5f5;
    padding: 1rem;
    border-radius: 8px;
  }

  ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  li {
    padding: 0.8rem 1rem;
    margin-bottom: 0.5rem;
    background-color: white;
    border-radius: 4px;
    cursor: pointer;
    transition: background-color 0.3s;
  }

  li:hover {
    background-color: #e0e0e0;
  }

  li:last-child {
    margin-bottom: 0;
  }
</style>