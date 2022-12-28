<template>
  <Container>
    <ChatWindow>
      <ChatMessage>
        </ChatMessage>
      </ChatWindow>
  </Container>
</template>
<script>
  import Container from "./components/MyContainer.vue";
  import ChatMessage from "./components/ChatMessage.vue";
  import ChatWindow from "./components/ChatWindow.vue";
  export default {
    name: "App",
    components: {
      Container,
      ChatMessage,
      ChatWindow,
    },
    data: () => ({
      messages: [],
    }),
    mounted() {
      this.loadMessage();
    },
    methods: {
      loadMessage() {
        this.axios
          .get("http://https://61bcd385d8542f0017824a2a.mockapi.io/messages")
      },
    }
  };

</script>
<style>
  body {
    margin: 0;
    background-color: #f9f9fa;
  }
</style>
