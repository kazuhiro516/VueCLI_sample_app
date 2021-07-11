<template>
  <div>
    <LikeHeader headerText="トータルのいいね数"></LikeHeader>
  </div>
</template>

<script>
import LikeHeader from "./components/LikeHeader.vue";

export default {
  data() {
    return {
      number: 14
    }
  },
  components: {
    LikeHeader: LikeHeader
  }
}
</script>
