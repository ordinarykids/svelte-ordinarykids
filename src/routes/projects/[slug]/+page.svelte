<script>
	export let data;
	console.log(data);
</script>


	<main class="basis-3/4 md:basis-3/3">
		<h1>blog post</h1>
	
			<img src={data.project.images[1]} alt={data.project.title} />
		
		<img src={data.project.image} alt={data.project.title} />
		<h1>{data.project.title}</h1>
		<div>{@html data.project.content}</div>
	</main>



