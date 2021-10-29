<template>
 <h1>{{title}}</h1> 
 <Modal :fordyBind="fordy" :textFordyBind="textfordy" themeProp="sale"/>
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: {
    Modal
  },
  data() {
     return {
        title:'My First Vue App :)',
        fordy: 'FOOOORRDD',
        textfordy: 'yeah lets try how this props works hahahah'
    }
  }
  
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1 {
  border-bottom: 1px solid #ddd;
  display: inline-block;
  padding-bottom: 10px;
}
</style>
