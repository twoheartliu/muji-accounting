<template>
  <nav>
    <router-link to="/money" class="item">
      <Icon type='money'/>
      记账
    </router-link>
    <router-link to="/labels" class="item">
      <Icon type="labels"/>
      标签
    </router-link>
    <router-link to="/statistics" class="item">
      <Icon type="statistics"/>
      统计
    </router-link>
  </nav>
</template>

<script lang="ts">
  export default {
    name: 'Nav'
  };
</script>

<style scoped lang="scss">
  nav {
    display: flex;
    box-shadow: 0 0 3px rgba(0, 0, 0, 0.85);
    flex-direction: row;
    font-size: 12px;

    > .item {
      width: 33.33333%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 2px 0;
    }

    .icon {
      width: 32px;
      height: 32px;
    }
  }

</style>