<template>
  <button>
    <slot :is-open="isOpen" />
  </button>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    }
  },

  methods: {
    open () {
      this.isOpen = true
    },
    close () {
      this.isOpen = false
    },
    toggle () {
      this.isOpen = !this.isOpen
    }
  }
}
</script>
