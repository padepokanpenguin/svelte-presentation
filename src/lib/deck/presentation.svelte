<script lang="ts">
	import Slide from './slide.svelte';
	import Code from './code.svelte';
    import Markdown from './markdown.svelte';
    import Notes from './notes.svelte';
</script>

<Slide animate>
	<Code lines>
		{function wellcome() {
			console.log('hai');
		}}
	</Code>
</Slide>

<Slide animate>
	<p class="text-red-600">Auto Animated</p>
</Slide>

<Slide animate>
	<p class="uppercase">Transtions</p>
	<div class="flex gap-2 place-content-center">
		<div data-id="box-1" class="w-[100px] h-[100px] bg-gray-400" />
		<div data-id="box-2" class="w-[100px] h-[100px] bg-gray-400" />
		<div data-id="box-3" class="w-[100px] h-[100px] bg-gray-400" />
	</div>
</Slide>

<Slide animate>
	<p class="uppercase">Transtions</p>
	<div class="flex gap-2 place-content-center">
		<div data-id="box-1" class="w-[200px] h-[200px] bg-red-400" />
		<div data-id="box-2" class="w-[200px] h-[200px] bg-green-400" />
		<div data-id="box-3" class="w-[200px] h-[200px] bg-blue-400" />
	</div>
</Slide>

<Markdown name="example.md" external />


<Slide>
    <h1>Slide note</h1>
    <Notes>Notes</Notes>
</Slide>

<Slide animate>
    <Slide>
        vertical 1
    </Slide>
    <Slide>
        vertical 2
    </Slide>
</Slide>