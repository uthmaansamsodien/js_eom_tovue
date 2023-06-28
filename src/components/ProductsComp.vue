<template>
    <div class="container">
        <div class="row">
            <div class="col" v-for="item in products" :key="item.ID">
        <div class="card" style="width: 18rem;">
            <img :src="item.image" class="card-img-top" :alt="item.model">
            <div class="card-body">
             <h1>{{item.brand}}</h1>
             <h2>{{item.model}}</h2>
             <h4>{{item.price}}</h4>
            </div>
          </div>
        </div>
        </div>
        </div>
</template>

<script>
export default {
        data(){
            return{
                data:[],
            }
        },
        methods:{
            async fetchData(){
                const res = await fetch('https://uthmaansamsodien.github.io/jsonserver3/user.json')
                let parsedData = await res.json()
                console.log(parsedData);
                let data = parsedData.products;
                console.log(data);
            },
        },
        mounted(){
                this.fetchData();
            },
    };
  
</script>

<style scoped>

</style>