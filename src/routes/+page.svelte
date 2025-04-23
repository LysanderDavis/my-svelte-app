<script lang="ts">
  import Nested from "./Nested.svelte";

  let inputValue = ""; // Variable to store input value

  function handleSubmit() {
    if (inputValue === "5") {
      alert("You are an idiot!");
    }
  }
</script>

<input type="text" bind:value={inputValue} placeholder="Enter a number" />
<button on:click={handleSubmit}>Submit</button>

<Nested />
