<template>
  <div id="app">
    <h2>Renderiza la lista de objectos del json</h2>
    <div v-for="(item,index) in json" :key="index">
      <h2>{{item.title}}</h2>
      <p>{{item.paragraph}}</p>
    </div>
  </div>
</template>

<script>
import json from './public/json/data.json'

export default {
  data() {
    return {
      json: json.data
    };
  }
}
</script>

<style>
</style>
