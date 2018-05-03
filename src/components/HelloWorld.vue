<template>
  <div>
    <button @click="clickButton">click button to emit</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  methods: {
    clickButton: function(val) {
      // $socket is socket.io-client instance
      this.$socket.emit("a", 12, 5);
    }
  }
};
</script>
