<template>
  <div>
    <LikeHeader>
      <template v-slot:title>
        <h2>こんにちは</h2>
      </template>
      <template v-slot:number>
        <p>{{number}}</p>
      </template>
    </LikeHeader>
    <div>
      <h2>イベントフォーム</h2>
      <label for="title">タイトル</label>
      <input
        id="title"
        type="text"
        v-model="eventData.title"
      >
      <p>{{ eventData.title }}</p>
    </div>
  </div>
</template>

<script>
import LikeHeader from "./components/LikeHeader.vue";

export default {
  data() {
    return {
      number: 14,
      eventData: {
        title: "タイトル"
      }
    }
  },
  components: {
    LikeHeader: LikeHeader
  }
}
</script>
