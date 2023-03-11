
<template>
  <div class="home">
    <h1> Shop for Sneakers </h1>
    <div class="products" v-for="product in products" :key="product.id">
      <img v-bind:src="product.image" width="200" >
     <div class="details"> 
      <router-link :to="{name: 'ProductDetails', params:{id: product.id}}"> 
        <h2> {{ product.title }} </h2>
      </router-link>
      
      <p> {{ product.details }} </p>
      <h3> Price: {{ product.price }} </h3> 
      <button @click="AddtoCart">Add to Cart</button>
     </div> 
     
    
    </div>

    

    
  </div>
</template>

<script>
export default {
  data(){
    return{
      products:[
        {title: 'Yeezy 700', id:1, details:'lorem', image:'YZY700.jpg', price:'Rs 15000' },
        {title: 'Yeezy Foam runner', id:2, details:'lorem', image:'YZYRNR.webp', price:'Rs 15000'  },
        {title: 'Yeezy 500 earth', id:3, details:'lorem', image:'YZY500.jpg', price:'Rs 15000'  },
      ]
      
    }
  },
  methdos: {
    AddtoCart(){
        
    }
  }
}
</script>

<style> 
   .products{
    text-align: left;
   }
   .products p{
    color:rgb(101, 101, 101);
   }
   .products .details{
    display:inline-block;
    text-align: left;
    padding:40px;
  }
  button{
    background: #e3e3e3;
    border:none;
    padding:10px;
    border-radius: 30px;
    transition-duration: 0.4s;
  }
  button:hover{
    background: #63d285;
  }
</style>
