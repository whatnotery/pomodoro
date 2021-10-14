<script>
	import TimeSet from "./timeSet.svelte";
</script>

<section id="container">
	<TimeSet timeType="work" />
	<TimeSet timeType="break" />
</section>

<style global lang="scss">
	@import "main.scss";

	#container {
		display: flex;
		flex-direction: row;
		justify-content: center;
	}
</style>
