<script>
export default {
    data() {
        return {
            iconBarBlu: [
                {
                    image: "/src/assets/img/buy-comics-digital-comics.png",
                    title: "digital comics"
                },
                {
                    image: "/src/assets/img/buy-comics-merchandise.png",
                    title: "dc merchandise"
                },
                {
                    image: "/src/assets/img/buy-comics-subscriptions.png",
                    title: "subscription"
                },
                {
                    image: "/src/assets/img/buy-comics-shop-locator.png",
                    title: "comic shop locator"
                },
                {
                    image: "/src/assets/img/buy-dc-power-visa.svg",
                    title: "dc power visa"
                },
            ]
        };
    },
    methods: {
        
    },
};
</script>

<template>
    <div class="sfondo-blu-iconbar">
        <div class="container-iconbar container-bg">
            <div v-for="(bar, index) in iconBarBlu" :key="index" class="card-icon">
                <div class="container-image">
                    <img :src="bar.image">
                </div>
                <div class="container-title">
                    <p>{{ bar.title }}</p>
                </div>
                
            </div>
        </div>
    </div>
</template>

<style scoped>
.sfondo-blu-iconbar{
    background-color: #057bf3;
    padding: 10px 0px;
}
.container-iconbar{
    display: flex;
    align-items: center;
    text-align: center;
    padding: 50px 0px;
}
.card-icon{
    width: 20%;
    display: flex;
    align-items: center;
    margin-right: 0px;
    
}
.container-image{
    width: 30%;
}
.container-image > img{
    width: 80%;
    text-align: start;
}
.container-title{
    width: 70%;
}
.container-title > p{
    text-transform: uppercase;
    font-size: 13px;
    text-align: start;
    margin-left: 5px;
    
}
</style>