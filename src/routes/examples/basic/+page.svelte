<script lang="ts">
	import Grid from '$lib';

	const items = [
		{ id: '0', x: 0, y: 0, w: 2, h: 5 },
		{ id: '1', x: 2, y: 2, w: 2, h: 2 },
		{ id: '2', x: 2, y: 0, w: 1, h: 2 },
		{ id: '3', x: 3, y: 0, w: 2, h: 2 },
		{ id: '4', x: 4, y: 2, w: 1, h: 3 },
		{ id: '5', x: 8, y: 0, w: 2, h: 8 },
		{ id: '6', x: 4, y: 5, w: 1, h: 1 },
		{ id: '7', x: 2, y: 6, w: 3, h: 2 },
		{ id: '8', x: 2, y: 4, w: 2, h: 2 }
	];
</script>

<Grid {items} cols={10} rows={10} let:item>
	<div class="item">{item.id}</div>
</Grid>

<style>
	.item {
		display: grid;
		place-items: center;
		background-color: rgb(150, 150, 150);
		width: 100%;
		height: 100%;
	}
</style>
