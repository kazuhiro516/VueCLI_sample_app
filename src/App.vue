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
      <p>{{ typeof eventData.maxNumber }}</p>
      <label for="maxNumber">テスト</label>
      <input
        id="title"
        type="text"
        v-model.trim="eventData.host"
      >
      <p>{{ typeof eventData.host }}</p>

      <label for="detail">イベントの内容</label>
      <textarea id="detail" cols="30" rows="10" v-model="detail"></textarea>
      <p>{{ eventData.detail }}</p>
      <input 
      type="checkbox"
      id="isPrivate"
      v-model="eventData.isPrivate"
      >
      <label for="isPrivate">非公開</label>
      <p>{{eventData.isPrivate}}</p>
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
        maxNumber: 0,
        host: "",
        detail: "",
        isPrivate: false
      }
    }
  },
  components: {
    LikeHeader: LikeHeader
  }
}
</script>
