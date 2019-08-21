<template>
<div>
    <h1>Product</h1>
    <div class="container">
        <div class="card-columns">
            <div class="card" v-for="prd in allproduct" :key="prd">
                <img class="card-img-top" :src="prd.image">
                <div class="card-body">
                    <h4 class="card-title">{{prd.id}} {{prd.name}}</h4>
                    <p class="card-text">{{prd.detail}}</p>
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
            // รายการสินค้า
            allproduct:[
                {
                    id:'1',
                    name:'Vue.Js',
                    price:'$22.39',
                    detail:'Vue.js is one of the latest new frameworks to have piqued the interest of web developers due to its reactivity, reusable components, and ease of use.',
                    image:'https://images-na.ssl-images-amazon.com/images/I/411MTXShkrL._SX403_BO1,204,203,200_.jpg'
                },
                {
                    id:'2',
                    name:'Vue.js 2 Cookbook',
                    price:'$22.39',
                    detail:'Vue.js is an open source JavaScript library for building modern, interactive web applications. With a rapidly growing community and a strong ecosystem, Vue.js makes developing complex single page applications a breeze. Its component-based approach, intuitive API, blazing fast core, and compact size make Vue.js a great solution to craft your next front-end application.',
                    image:'https://images-na.ssl-images-amazon.com/images/I/413yu7uDunL._SX403_BO1,204,203,200_.jpg'
                },
                {
                    id:'3',
                    name:'Vue.js Component Patterns',
                    price:'$9.99',
                    detail:'This book is a quick and fun read that will teach you advanced component patterns with Vue.js!',
                    image:'https://images-na.ssl-images-amazon.com/images/I/31SIuIVad7L.jpg'
                },
            ]
        }
    }

}
</script>

<style>
div .card img {
    /* width: 200px; */
    margin: auto;
    width: 50%;
    padding: 10px;
}
</style>
