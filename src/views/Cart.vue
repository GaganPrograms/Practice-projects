<template>
<div> 
    <h1> Shopping Cart </h1>
    <div class="items" v-for="item in userarray" :key="item.id"> 
        <!-- <h3> {{ item.title }} </h3> -->
        
    </div>
     
</div>
</template>

<script>
export default{
    


    data(){
        return{
            userarray:[
      {title: 'Yeezy 700 vanta black', id:1, details:'lorem', image:'logo.png', price:'Rs 15000' },
      {title: 'Yeezy Foam runner', id:2, details:'lorem', image:'logo.png', price:'Rs 15000'  },
        
      ]
        }
    }
    // methods:{
    //     addtocarthere(product){
    //         userarray.concat(product)
    //     }
    // }
    
   
}
</script>


<style> 

</style>