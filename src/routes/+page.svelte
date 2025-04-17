<script lang="ts">
  import Nested from "./Nested.svelte";
  let numbers = $state([1,2,3,4]);

  function addNumber() {
    numbers.push(numbers.length + 1);
  }
</script>

<p>{numbers.join(' + ')} = ...</p>

<button onclick={addNumber}>
  Add a number
</button>

<Nested />
