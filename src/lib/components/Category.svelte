<script>
    let {data, cwd} = $props();

    import Grid from "$lib/components/Grid.svelte";
</script>

<style>
.inner {
    width: 100%;
}
</style>

<div class="inner" style={`rgb(${r(0, 255)}, ${r(0, 255)}, ${r(0, 255)});`}>
<h1>{cwd}</h1>

<!-- definitely a better way to do this other than cwd as a prop -->
<Grid data={data} cwd={cwd}></Grid>
</div>