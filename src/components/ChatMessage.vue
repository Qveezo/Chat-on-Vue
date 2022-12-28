<template>
  <div class="chat-message">
    <div class="info">{{ username }} {{ datetime }}</div>
  </div>
</template>
<script>
export default {
  name: "ChatMessage",
  props: {
    username: String,
    datetime: String,
    },
  };
</script>
<style>
  .chat-message {
    font-family: "Arial", sans-serif;
    font-size: 16px;
    padding: 15px 20px;
    border-radius: 20px;
    background: #fff;
    border: 1px solid #eee;
    box-shadow: 0 3px 5px 0 #5f5f5f73;
    color: #16a085;
    margin-bottom: 15px;
  }
  .chat-message .info {
    color: #78909c;
    font-size: 13px;
    margin-bottom: 5px;
  }
</style>
