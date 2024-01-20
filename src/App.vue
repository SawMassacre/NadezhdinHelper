<template>
  <HelloWorld />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
@font-face {
  font-family: "NEXT ART";
  src: url("./assets/NEXT ART_Regular.otf") format("truetype");
}

@font-face {
  font-family: "NEXT ART";
  src: url("./assets/NEXT ART_Bold.otf") format("opentype");
  font-weight: bold;
}

@font-face {
  font-family: "NEXT ART";
  src: url("./assets/NEXT ART_SemiBold.otf") format("opentype");
  font-weight: 600;
}

body {
  font-family: "NEXT ART", sans-serif;
}

strong {
  font-weight: bold;
}

.semi-bold {
  font-weight: 600;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
