<script>

export default{

  data() {
    return {
      navBar: [
        {
          text: "characters",
          url: "#"
        },
        {
          text: "comics",
          url: "#"
        },
        {
          text: "movies",
          url: "#"
        },
        {
          text: "tv",
          url: "#"
        },
        {
          text: "games",
          url: "#"
        },
        {
          text: "collectibles",
          url: "#"
        },
        {
          text: "videos",
          url: "#"
        },
        {
          text: "fans",
          url: "#"
        },
        {
          text: "news",
          url: "#"
        },
        {
          text: "shop",
          url: "#"
        },
      ]
    }
  },
  methods: {
    
  },
  
}

</script>

<template>
  <header>
    <div class="container-testata container-bg">
      <div class="container-img">
        <img src="../assets/img/dc-logo.png">
      </div>
      <div class="container-navbar">
        <span v-for="(nav, index) in navBar" :href="nav.url" :key="index">{{ nav.text }}</span>
      </div>
    </div>
    
  </header>
</template>

<style scoped>

.container-testata{
  display: flex;
  align-items: center;

}
header{

  background-color:white;
  padding: 20px 0px;
}
span{
  color: black;
  margin-right: 30px;
  text-transform: uppercase;
  font-size: 11px;
  font-weight: 600;
}
.container-img{
  width: 100%;
} 
.container-img > img{
  width: 25%;
} 
.container-navbar{
  width: 75%;
}

</style>
