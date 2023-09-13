<script>
	export let data;
</script>


<h1>blog</h1>
<p class="text-sm hover:text-base">
asdasd
</p>


<div class="grid grid-cols-2 gap-4">

	<div class="card">
		<!-- card content -->asdasdasd
	</div>

	<div class="card">
		<!-- card content -->asda
	</div>

	<div class="card">
		<!-- card content -->asdasd
	</div>

	<div class="card">
		<!-- card content -->asdasd
	</div>

</div>


<ul>

	{#each data.summaries as { slug, title }}
		<li><a href="/projects/{slug}">{slug}</a></li>
	{/each}
</ul>