<template>
 <ul>
    <li v-for="category in categories" :key="category.slung">
    <n-link
     :to="{
        name: 'categories-slung',
        params:{slung:category.slung}
     }">
     
      <category-view :category="category"></category-view>
     </n-link>
    </li>
  </ul> 
</template>

<script>
  export default{
    props:["categories"],
  };
</script>
