<template>
    {}
</template>

<script>
import requests from './request';
export default{
data(){
    return{
    data:[],
}
},
methods:{
    async getAllCountries(){
       const response= fetch(request.getAllCountries);
       this.data= await response.json();
    }
}
</script>
 