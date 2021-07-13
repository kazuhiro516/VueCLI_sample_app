<template>
  <div>
    <LikeHeader>
      <h1>トータルのいいね数</h1>
      <h2>{{number}}</h2>
    </LikeHeader>
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
