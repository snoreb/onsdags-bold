<!-- App.svelte -->
<script>
	import CardComponent from '../components/CardComponent.svelte';
	import { players } from '$lib/players';
	// Example list of card data
	let cards = players;


</script>


	<div class="content">
		<div class="card-container">
			{#each cards as { img, title, uniDegree, stats }}
				<div class="card-wrapper">
					<CardComponent {img} {title} {uniDegree} {stats} />
				</div>
			{/each}
		</div>
	</div>

<style>


	.card-container {
		display: flex;
		flex-wrap: wrap;
		gap: 16px; /* Adds space between the cards */
		justify-content: center; /* Aligns items to the start */
		max-width: 40vw; /* Ensure container takes up max 70% of viewport width */
		margin: 0 auto; /* Center container horizontally */
	}

	.card-wrapper {
		margin-top: 10px;
		flex: 1 1 calc(100% - 16px); /* Width of each card */
		max-width: calc(100% - 16px); /* Width with gap considered */
		box-sizing: border-box;
	}

	.card-img {
		width: 100%; /* Ensure the image takes up the full width of the card */
		height: 150px; /* Set a fixed height for the image */
		object-fit: cover; /* Maintain aspect ratio and cover the area */
	}
</style>
