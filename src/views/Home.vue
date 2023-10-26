<script setup>
    import InputBox from "@/components/InputBox.vue"

    function submitForm () {
        console.log("hola")
    }

</script>

<template>
  <main>
      <form @submit.prevent="submitForm">
          <InputBox label="Capital" type="number"/>
          <InputBox label="Tasa De Interes" type="number"/>
          <InputBox label="Periodo" type="number"/>

          <!-- dias años meses -->
          <!-- <RadioBox /> -->
          <InputBox label="Dias" type="radio" value="days" name="periodo"/>
          <InputBox label="Meses" type="radio" value="months" name="periodo"/>
          <InputBox label="Años" type="radio" value="years" name="periodo"/>

          <input type="submit" value="Calcular">
      </form>
  </main>
</template>

