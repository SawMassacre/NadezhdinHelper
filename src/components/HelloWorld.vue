<template>
  <div class="main__logo semi-bold" style="margin: 0.5em">
    <p class="header__title">Надеждин</p>
    <p class="header__subtitle">2024</p>
  </div>
  <div class="page-container">
    <h1 style="width: 40vw; text-align: center">
      Это приложение поможет тебе заполнять бланки правильно
    </h1>
    <h2 style="width: 45vw; text-align: center">
      Чтобы проверить как сокращается какое либо слово просто впиши его в поле
      внизу👇🏻
    </h2>
    <div class="input-container">
      <input
        type="text"
        v-model="inputValue"
        placeholder="Введите текст здесь"
        class="form__input form__input--centered"
      />
    </div>
    <h1>Правильно будет так:</h1>
    <div class="output-container">
      <div
        class="form__output form__output--centered"
        style="height: 3em; width: 18em"
      >
        {{ abbreviation }}
      </div>
    </div>
  </div>
</template>

<script>
const dictionary = {
  город: "г.",
  "городской округ": "г.о.",
  "городское поселение": "г.п.",
  "сельское поселение": "с.п.",
  район: "р-н",
  село: "с.",
  поселок: "п.",
  "поселок городского типа": "пгт.",
  деревня: "д.",
  станица: "ст-ца",
  хутор: "х.",
  бульвар: "б-р",
  квартал: "кв-л",
  микрорайон: "мкр.",
  набережная: "наб.",
  переулок: "пер.",
  площадь: "пл.",
  проезд: "пр-д",
  проспект: "просп.",
  улица: "ул.",
  шоссе: "ш.",
  дом: "д.",
  корпус: "к.",
  строение: "стр.",
  квартира: "кв.",
  комната: "ком.",
};

function getAbbreviation(word) {
  return dictionary[word];
}

export default {
  data() {
    return {
      inputValue: "",
    };
  },
  computed: {
    abbreviation() {
      return getAbbreviation(this.inputValue);
    },
  },
};
</script>

<style scoped>
.main__logo {
  background-image: url("../assets/streak-8a1963b3.webp");
  background-repeat: no-repeat;
  background-size: cover;
  background-size: 90%;
  font-family: NEXT ART, sans-serif;
  font-weight: 600;
  font-size: 1.5625em;
  text-decoration: none;
  line-height: 0.85;
  color: currentColor;
  letter-spacing: -0.05em;
  padding: 0.75em 0.5em 0.75em 0;
  margin-right: 1.75em;
  display: inline-block;
  position: relative;
}
.header {
  text-align: left;
  font-weight: 600;
  font-size: 1.5625em;
  text-decoration: none;
  line-height: 0.85;
  color: currentColor;
  letter-spacing: -0.05em;
  padding: 0.75em 0.5em 0.75em 0;
  margin-right: 1.75em;
  display: inline-block;
  position: relative;
}
.form__output {
  text-align: center;
}

.form__output--centered {
  font: inherit;
  font-size: inherit;
  font-size: 0.875em;
  text-transform: uppercase;
  display: block;
  width: 100%;
  border-width: 0;
  padding: 1em;
}
.form__input--centered {
  text-align: center;
}

.form__input {
  font: inherit;
  font-size: inherit;
  font-size: 0.875em;
  text-transform: uppercase;
  display: block;
  width: 100%;
  height: 3em;
  width: 18em;
  border-width: 0;
  padding: 1em;
}

.output-container {
  background: #d4e5f0;
  display: flex;
  padding: 2em;
  border-radius: 0.5em;
}

.input-container {
  background: #d4e5f0;
  display: flex;
  padding: 2em;
  border-radius: 0.5em;
}
.page-container {
  gap: 2em;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 70vh;
  font-family: "NEXT ART", sans-serif;
}
</style>
