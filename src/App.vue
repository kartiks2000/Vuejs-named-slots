<template>
  <div class="kk">
    <h1>Hello!! I am the parent....</h1>
    <Child>
      <h1 slot="main-text">how are you???</h1>
      <h2 slot="secondry-text">i am {{post}}</h2>
      <h1 slot="tertiary-text">good....</h1>
    </Child>
  </div>
</template>

<script>
import child from './child';
export default {
  components:{
    Child : child,
  },
  data:() => {
    return {
      post : "product manager"
    }
  }
}
</script>

<style scoped>
  h1{
    color: red;
  }
  div{
    margin: 3rem;
  }
  .kk{
    background-color: cornsilk;
    padding: 3rem;
  }
</style>>
