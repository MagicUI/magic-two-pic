<template>
  <div id="app">
    <index :moduleInfo="moduleInfo"></index>
  </div>
</template>

<script>
import Index from './components/index.js';
import SchemaData from './schema.json';
export default {
  name: 'app',
  components: {
    Index
  },
  data() {
      return {
          moduleInfo: {
            name: '双图模块',
            type: 'two-pic',
            schema: SchemaData
          }
      }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
