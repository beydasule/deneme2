<template>
<div class = "container">
  <!--myComp /> --> 
  <Product :product = "product" v-for = "product in productList" :key = "product.id" />
  
</div>
</template>

<script>
//import MainContainer from "@/components/MainContainer"
import Product from "@/components/Product"
export default {
  components : {
    //myComp : MainContainer,
    Product
  },
  data(){
    return{
      productList : [
                    {
                        id : 1,
                        title : "MacBook Pro22",
                        price : 100,
                        count : 10,
                        description : "Açıklama 1"
                    },
                    {
                        id : 2,
                        title : "iPhone",
                        price : 50,
                        count : 100,
                        description : "Açıklama 2"
                    },
                    {
                        id : 3,
                        title : "Klavye",
                        price : 10,
                        count : 1000,
                        description : "Açıklama 3"
                    }
                ]
    }
  }
  
}
</script>


<style>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

</style>