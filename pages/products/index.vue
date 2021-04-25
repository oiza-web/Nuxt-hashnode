<template>
<div>
  <h1>My Products</h1>
  <input type="text" v-model="productId">
  <button @click="loadProduct">Choose Product</button>
</div>

</template>
<script>
export default {
  data(){
    return{
      productId : ''
    }
  },
  methods:{
    loadProduct(){
      this.$router.push('/products/' + this.productId)
    }
  }
}
</script>

<style scoped>
button{
  background-color: black;
  color: white;
  border: none;
  padding: 8px;
  border-radius: 3px;
  cursor: pointer;
}

input {
  width: 180px;
  height: 30px;
  margin-top: 2%;
}
</style>
