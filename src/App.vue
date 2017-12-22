<template>
  <div>
    <popper trigger="click" :options="{placement: 'top'}">
      <div class="popper">
        Popper Content
      </div>

      <button slot="reference">
        Popper Element (Click)
      </button>
    </popper>

    <span title="tippy tooltips" v-tippy>Tooltip Element (Hover)</span>
  </div>
</template>

<script>
  import Popper from 'vue-popperjs'
  import 'vue-popperjs/dist/css/vue-popper.css'

  export default {
    components: {
      'popper': Popper
    }
  }
</script>
