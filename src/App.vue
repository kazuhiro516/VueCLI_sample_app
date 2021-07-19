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
      <label for="maxNumber">最大人数</label>
      <input
        id="title"
        type="number"
        v-model.number="eventData.maxNumber"
      >
      <p>{{ typeof eventData.maxNumber }}</p>
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
        title: "タイトル",
        maxNumber: 0
      }
    }
  },
  components: {
    LikeHeader: LikeHeader
  }
}
</script>
