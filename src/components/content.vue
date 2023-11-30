<script>

export default{
    props: ["fumetti"]

}

</script>


<template>
    <div class="container-content">
        <div class="container-bg">
            <p class="background-blue">Current Series</p>
        </div>
        
        <div class="container-bg flex">
            <div v-for="(fumetto, index) in fumetti" :key="index" class="card-fumetti">
                <img :src="fumetto.thumb">
                <h5>{{ fumetto.series }}</h5>
                
            </div>
        </div>
        <button class="button">Load More</button>
    </div>
 
</template>


<style scoped>
.container-content{
    min-height:auto;
    background-color: #1a1a1a;
    text-align: center;
    margin-top: -25px;
   
}
h1{
    margin: 0;
}
h3{
    color: white;
}
.flex{
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: space-between;
}
.card-fumetti{
    
    width: 15%;
}
.card-fumetti > img{
   width: 100%;
   height: 150px;
   object-fit: cover;
   object-position: top;
}
h5{
    text-align: start;
}
.background-blue{
    background-color: #057bf3;
    width: 15%;
    padding: 10px 20px ;
    text-transform: uppercase;
    text-align: start;
    margin: 0px 0px 20px 0px;
    font-weight: 600;
    z-index: 99;
    position: relative;
    
}
</style>