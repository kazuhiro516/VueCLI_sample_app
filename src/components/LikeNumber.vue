<template>
  <p>いいね({{number}})</p>
</template>

<script>
export default {
  props: ["number"],
  data: function() {
    return {
      number: 5
    };
  }
}
</script>
