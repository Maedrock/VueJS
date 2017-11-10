<template>
    <header id="ht">
        <h1>{{ title }}</h1>
    </header>
</template>

<script>
export default {
  data() {
    return {
      title: "Halloween Album"
    };
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Poiret+One");
#ht {
  font-family: "Poiret One", cursive;
}
header {
  background-color: rgb(58, 48, 66);
  padding: 10px;
}
h1 {
  color: rgba(219, 157, 71, 0.9);
  text-align: center;
  border-bottom: 5px solid rgba(190, 187, 187, 0.8);
  padding-bottom: 10px;
}
#idCont {
  background-color: rgb(58, 48, 66);
}
img {
  display: block;
  position: relative;
}
</style>