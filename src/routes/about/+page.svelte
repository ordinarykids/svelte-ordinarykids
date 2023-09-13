<script>

	import { Swipe, SwipeItem } from "svelte-swipe";
	import Project from "$lib/project.svelte";
	const swipeConfig = {
		autoplay: false,
		delay: 2000,
		showIndicators: true,
		transitionDuration: 400,
		defaultIndex: 0,
		allowInfiniteSwipe: true,
	};
</script>

<style>
	.swipe-holder{
		height: 90vh;
		width: 100vw;
		background-color: aqua;
	}
	img{
		max-width: 100vw;
		width: 50vw;
		height: auto;
		margin: 10vh auto;
	}
	h1 {
		font-size: 10vh;
	}

	.page-header {
		text-align: center;
		position: fixed;
		z-index: 100;
	}
</style>
<div class="page-header">
	<h1>ABOUT ORDINARYKIDS</h1>
	<Project projectId='2' />
</div>

<div class="swipe-holder">
	<Swipe {...swipeConfig}>
		<SwipeItem allow_infinite_swipe={true}>
			<img src="./undertrains.jpg" alt="">
		</SwipeItem>

		<SwipeItem>
			<img src="./images/n2.jpg" alt="">
		</SwipeItem>

		<SwipeItem>
			<img src="./images/n3.jpg" alt="">
		</SwipeItem>

		<SwipeItem>
			<img src="./images/n4.jpg" alt="">
		</SwipeItem>
	</Swipe>
</div>


<div class="swipe-holder">
	<Swipe {...swipeConfig}>
		<SwipeItem>
			<img src="./images/n1.jpg" alt="">
		</SwipeItem>

		<SwipeItem>
			<img src="./images/n2.jpg" alt="">
		</SwipeItem>

		<SwipeItem>
			<img src="./images/n3.jpg" alt="">
		</SwipeItem>

		<SwipeItem>
			<img src="./images/n4.jpg" alt="">
		</SwipeItem>
	</Swipe>
</div>