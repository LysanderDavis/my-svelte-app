<script lang="ts">
  import Nested from "./Nested.svelte";

  let numbers = $state([1, 2, 3, 4]);
  let total = $derived(numbers.reduce((t, n) => t + n, 0));
  let sum = $derived(numbers.reduce((t, n) => t + n, 0) );
  function addNumber() {
    numbers.push(numbers.length + 1);
  }
</script>

<p>{numbers.join(' + ')} = {total}</p>

<button onclick={addNumber}>
  Add a number
</button>

<Nested />