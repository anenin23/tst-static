<script setup lang="ts">
const doSomething = () => {
  alert('doSomething')
}

const attrName = 'href2'
const attrValue ='/'
</script>


<template>
  <div class="about">
    <h1>This is an about page</h1>
    <a :[attrName]="attrValue" @click.prevent="doSomething">do something </a>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
