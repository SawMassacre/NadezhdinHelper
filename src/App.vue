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
  background-color: #fff;
  opacity: 1;
  background-image: linear-gradient(#d4e5f0 2.6px, transparent 2.6px),
    linear-gradient(to right, #d4e5f0 2.6px, #fff 2.6px);
  background-size: 52px 52px;
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

@media screen and (max-width: 1366px) {
  body {
    font-size: 13px;
  }
}
@media screen and (max-width: 1100px) {
  body {
    font-size: 12px;
  }
}
@media screen and (max-width: 960px) {
  body {
    font-size: 16px;
  }
}
@media screen and (max-width: 480px) {
  body {
    font-size: 14px;
  }
}
@media screen and (max-width: 410px) {
  body {
    font-size: 12px;
  }
}

@media screen and (max-width: 1366px) {
  h1 {
    font-size: 1.5em;
  }
  h2 {
    font-size: 1.4em;
  }
  h3 {
    font-size: 1.1em;
  }
}

@media screen and (max-width: 1100px) {
  h1 {
    font-size: 1.5em;
  }
  h2 {
    font-size: 1.4em;
  }
  h3 {
    font-size: 1.1em;
  }
}

@media screen and (max-width: 960px) {
  h1 {
    font-size: 1.5em;
  }
  h2 {
    font-size: 1.4em;
  }
  h3 {
    font-size: 1.1em;
  }
}

@media screen and (max-width: 480px) {
  h1 {
    font-size: 1.5em;
  }
  h2 {
    font-size: 1.4em;
  }
  h3 {
    font-size: 1.1em;
  }
}

@media screen and (max-width: 410px) {
  h1 {
    font-size: 1.5em;
  }
  h2 {
    font-size: 1.4em;
  }
  h3 {
    font-size: 1.1em;
  }
}

h1,
h2,
h3 {
  background-color: #d4e5f0;
  border-radius: 0.5em;
  padding: 0.1em;
}
</style>
