<template>
  <Defog
    maxWidth="100%"
    maxHeight="100%"
    apiEndpoint="https://test-defog-ikcpfh5tva-uc.a.run.app"
    buttonText="Ask Defog"
    darkMode=false
  />
</template>

<script>
import { applyReactInVue } from 'vuereact-combined'
import { AskDefogChat } from "defog-components"
export default {
  components: {
    // Use HOC 'applyReactInVue'
    Defog: applyReactInVue(AskDefogChat)
  }
}
</script>