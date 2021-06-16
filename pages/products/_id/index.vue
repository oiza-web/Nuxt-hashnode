<template>
  <h1>Product with ID : {{ $route.params.id}}</h1>
</template>
<script>
export default {
  validate(data){
    return data.params.id == 1
  }
}
</script>
