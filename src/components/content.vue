<script>

export default{
    props: ["fumetti"]

}

</script>


<template>
    <div class="container-content" >
        <div class="container-bg">
            <div v-for="(fumetto, index) in fumetti" :key="index">
                <img :src="fumetto.thumb">
                <h3>{{ fumetto.series }}</h3>
            </div>
        </div>
    </div>
 
</template>


<style scoped>
.container-content{
    height: 150px;
    background-color: black;
    display: flex;
    align-items: center;
}
h1{
    margin: 0;
}
h3{
    color: white;
}


</style>