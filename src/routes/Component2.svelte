<script lang="ts">
	import type { Snippet } from 'svelte';

	type Props = {
		someSnippet?: Snippet;
	};

	let { someSnippet }: Props = $props();
</script>

{#if someSnippet}
	{@render someSnippet()}
{:else}
	<span>NO SNIPPET PASSED</span>
{/if}
