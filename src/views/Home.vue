<template>
    <div>
        <p style="text-align: center">Welcome to Nota!</p>
        <div id="editorjs">

        </div>
    </div>
</template>
<script lang="ts">
import EditorJS from '@editorjs/editorjs'; 
import { onMounted } from '@vue/runtime-core';

export default {
    setup() {
        onMounted(()=>{
            (Window as any).editor = new EditorJS('editorjs')
        })
    }
}
</script>