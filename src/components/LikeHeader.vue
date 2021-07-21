<template>
  <slot name="title"></slot>
  <hr>
  <p>いいね</p>
  <slot name="number"></slot>
</template>

<script>
export default {
  props: ["headerText"]
}
</script>
