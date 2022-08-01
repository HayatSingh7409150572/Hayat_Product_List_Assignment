<template>
    <div>
        <pre>{{JSON.stringify(merchant,null,2)}}</pre>
        <category-list :categories="categories"></category-list>
        <product-list :products="products"></product-list>
    </div>
</template>

<script>
import commerce from '~/common/commerce'
export default{

async asyncData(){
  const merchant = await commerce.merchants.about()
  const {data:categories} =  await commerce.categories.list()
  const {data:products} = await commerce.products.list();

  return {
    merchant,
    categories,
    products
  }
 }
}

</script>