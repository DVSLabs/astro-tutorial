<script>
  export let messages;
  let greeting = messages[0];

  function randomMessage() {
    greeting = messages[Math.floor(Math.random() * messages.length)];
  }
</script>

<div>
  <h3>{greeting}! Thank you for visiting!</h3>
  <button on:click={randomMessage}> New Greeting </button>
</div>
