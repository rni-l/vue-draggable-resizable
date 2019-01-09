<template>
  <div id="app">
    <div style="height: 500px; width: 500px; border: 1px solid red; position: relative;">
      <vue-draggable-resizable :w="400" :h="400" :parent="true" :debug="false" :isParentOfWindow="true"
        classNameHandle='test' className='test-ttt'
        :min-width="200" :min-height="200">
        <p>vue-draggable-resizable</p>
      </vue-draggable-resizable>
    </div>
  </div>
</template>

<script>
import VueDraggableResizable from './components/vue-draggable-resizable'
// import './components/vue-draggable-resizable.css'

export default {
  name: 'app',
  components: {
    VueDraggableResizable
  }
}
</script>

<style>
  .vdr {
    /* border: 1px dashed black; */
  }
  *{margin: 0;padding: 0;}
  html, body {
    width: 100%;
    height: 100%;
  }
</style>
