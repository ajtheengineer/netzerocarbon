<script setup lang="ts">
  import WelcomeItem from './WelcomeItem.vue'
  import DocumentationIcon from './icons/IconDocumentation.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Why?</template>

    <p>
      Electric vehicles may not yet be the best for the environment yet. It depends on the make/model of the car, size of the battery, and how electricity is generated in your region.
    </p>
    <br />
    <p>
     This tool is to show you the lifetime carbon footprint of your vehicle, which includes both up-front the carbon footprint of the production process and carbon emitted over time as the car mileage increases.
    </p>
    <br />
    <p>
      This website is inspired from this <a target="_blank" href="https://youtu.be/S1E8SQde5rk">Ted Talk by Graham Conway.</a>
    </p>
  </WelcomeItem>

</template>
