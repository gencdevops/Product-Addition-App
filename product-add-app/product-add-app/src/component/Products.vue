<template>
  <div class="row product-container">

  <appProduct v-for="product in productList">
    <img class="card-img-top" src="/src/assets/default.png" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card title</h5>
      <small>
        <strong>Adet : </strong> 1
      </small>
      <br>
      <small>
        <strong>Fiyat : </strong> 10
      </small>
      <br>
      <small>
        <strong>Tutar : </strong> 10
      </small>
    </div>
  </appProduct>

  </div>
</template>

<script>
import Product from "./Product";
export default {
  name: "Products",
  components : {
    appProduct : Product
  },
  data() {
    return {
      productList : [],
    }
  }
}
</script>

<style scoped>

</style>