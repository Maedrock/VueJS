<template>
    <div id="amorph">
        <ul>
            <li v-for="info in infos" v-bind:key="info.show">
                <h1 v-on:click="info.show = !info.show">{{ info.name }}</h1>
                <h2 v-show="info.show">└ {{ info.role }} ({{ info.age }})</h2>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    props:{
        infos: {
            type: Array,
            required: true
        }
    },
  data() {
    return {

    };
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Poiret+One");
#amorph{
    font-family: "Poiret One", cursive;
    background-color: rgb(58, 48, 66);
    color:  rgb(229, 234, 250);
    margin: 0px;
    text-align: center;
}
ul{
    width: auto;
    padding: 0;
}
li{
    list-style: none;
    background: rgb(219, 157, 71);
    margin-bottom: 5px;
}
li h1{
    padding-left: 5px;
}
li h2{
    background: rgb(58, 48, 66);;
    margin:0;
    padding: 5px 0 0 10px;
    color: #F1F5F2;
}
li h2 span{
    color:rgb(58, 48, 66);
    font-weight: normal;
    font-style: italic;
    font-size: 15px;
}
li p{
    margin-top: 2px;
    padding: 5px;
    font-size: 18px;
}
p span{
    font-weight: 700;
}
</style>
 