<template>
  <div id="app">
    <tiptap />
  </div>
  <p>Using text interpolation: {{ rawHtml }}</p>
  <p>Using v-html directive: <span v-html="rawHtml"></span></p>
</template>

<script>
  import Tiptap from './components/Tiptap.vue'
  export default {
    name: 'App',
    components: {
      Tiptap,
    },
    data() {
      return {
        rawHtml: '<span style="color: red;">这是红色文本</span>'
      }
    },
  }
</script>

