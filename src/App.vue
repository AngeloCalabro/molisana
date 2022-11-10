<template>
<HeaderComponent/>
<main>
<ProductList/>
</main>
<FooterComponent/>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import ProductList from './components/ProductList.vue';
import FooterComponent from './components/FooterComponent.vue';
  export default {
    components: { HeaderComponent, ProductList, FooterComponent }
}
</script>

<style lang="scss" scoped>

</style>