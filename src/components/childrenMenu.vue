<template>
  <ul>
    <li v-for="childs in childrens" :key="childs.id">
      <router-link :to="'/' + childs.id">
        <p>{{ childs.name }}</p>
      </router-link>
    </li>
  </ul>
</template>

<script>
  export default {
    props: ['childrens']
  }
</script>

<style lang="scss" scoped>

</style>