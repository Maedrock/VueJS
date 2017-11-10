<template>
    <footer id="ht">
        <p>{{ copyright}}</p>
    </footer>
</template>

<script>
export default {
  data() {
    return {
      copyright: "github.com/Maedrock"
    };
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Poiret+One");
#ht {
  font-family: "Poiret One", cursive;
  margin-top: -5px;
}
footer {
  background-color: rgba(58, 48, 66, 0.9);
  padding: 7px;
  font-size: 20px;
}
p {
  color: rgb(219, 157, 71);
  text-align: center;
}
</style>