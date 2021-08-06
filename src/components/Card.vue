<template>
  <li class="card">
    <div class="p-3">
      <p>{{ text }}</p>
    </div>
  </li>
</template>

<script>
import { reactive, toRefs } from 'vue'

export default {
  props: {
    text: {
      type: String,
    },
  },
  setup() {
    // console.log(props.text)
    const state = reactive({})

    return {
      ...toRefs(state),
    }
  },
}
</script>
