<script lang="ts">
	import Component1 from './Component1.svelte';
</script>

<Component1 value={1}>
	<span slot="placeholder"></span>
</Component1>

<hr />

<Component1 value={2}>
	<span slot="placeholder"></span>
</Component1>
