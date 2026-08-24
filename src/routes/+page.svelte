<script lang="ts">
	const tools = [
		{ name: 'sendme', link: 'https://www.iroh.computer/sendme' },
		{ name: 'Tool 2', link: '/tools/tool2' },
		{ name: 'Tool 3', link: '/tools/tool3' }
	];
</script>

<div class="flex min-h-screen flex-col p-4">
	<h2>
		<span class="text-3xl font-bold">Frkri.dev</span>
	</h2>

	<ul class="mt-4">
		{#each tools as tool (tool.name)}
			<li class="text-lg font-bold">
				<a href={tool.link} rel="external">{tool.name}</a>
			</li>
		{/each}
	</ul>
</div>
