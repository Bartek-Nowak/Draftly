<template>
  <div ref="editorContainer" style="height: 500px;" />
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'
import '@toast-ui/editor/dist/toastui-editor.css'
import Editor from '@toast-ui/editor'

const editorContainer = ref(null)
let editorInstance = null

onMounted(() => {
  editorInstance = new Editor({
    el: editorContainer.value,
    height: '500px',
    initialEditType: 'markdown',
    previewStyle: 'vertical'
  })
})

onBeforeUnmount(() => {
  if (editorInstance) {
    editorInstance.destroy()
  }
})
</script>
