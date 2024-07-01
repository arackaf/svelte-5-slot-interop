<script lang="ts">
	import Component2 from './Component2.svelte';

	const { value }: { value: any } = $props();
</script>

<Component2>
	{#if $$slots.placeholder}
		{#snippet renderPlaceholder()}
			<span>Slot was passed - rendering below</span>
			<slot name="placeholder" slot="placeholder"></slot>
		{/snippet}
	{/if}
</Component2>
