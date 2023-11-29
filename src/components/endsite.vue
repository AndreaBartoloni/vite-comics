<script>

export default{

    data() {
  return {
    contentFooter: {
      dcComics: [
        {
          titleFooter: "dc comics",
        },
        {
          text: "characters",
        },
        {
          text: "Comics",
        },
        {
          text: "Movies",
        },
        {
          text: "Tv",
        },
        {
          text: "Games",
        },
        {
          text: "Videos",
        },
        {
          text: "News",
        },
      ],
      dcComics: [
            {
            titleFooter: "dc comics",
            },
            {
            text: "characters",
            },
            {
            text: "Comics",
            },
            {
            text: "Movies",
            },
            {
            text: "Tv",
            },
            {
            text: "Games",
            },
            {
            text: "Videos",
            },
            {
            text: "News",
            },
        ],
      // Altri tipi di footer o ulteriori dati possono essere aggiunti qui
    },
  };
},

    methods: {
        
    },
}


</script>


<template>
    <div class="container-footer-image">
        <div class="big-logo">
            <!-- <img src="../assets/img/dc-logo-bg.png"> -->
            <div class="container-bg">
                <div v-for="(contentF, index) in contentFooter" :key="index">
                    <div v-for="(item, index) in contentF" :key="index">
                        <h4>{{ item.titleFooter }}</h4>
                        <p>{{ item.text }}</p>
                    </div>
                 
                </div>
            </div>
        </div>
   </div>
</template>


<style scoped>

.container-footer-image{
    background-image: url(../assets/img/footer-bg.jpg);
    min-height: auto;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
.big-logo{
    background-image: url(../assets/img/dc-logo-bg.png);
    height: 500px;
    background-position: right;
    background-repeat: no-repeat;
    background-size: contain;
    background-position-x: 700px;
}
h4{
    text-transform: uppercase;
}
p{
    line-height: 0.5em;
}

</style>