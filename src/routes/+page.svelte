<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->
<script lang="ts">
	import Hero from "$lib/Hero.svelte";
	import { Avatar } from "@skeletonlabs/skeleton";
</script>

<Hero/>

<!--
<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-5">
		<h1 class="h1">Let's get cracking bones!</h1>
		<p>Start by exploring:</p>
		<ul>
			<li><code class="code">/src/routes/+layout.svelte</code> - barebones layout</li>
			<li><code class="code">/src/app.postcss</code> - app wide css</li>
			<li>
				<code class="code">/src/routes/+page.svelte</code> - this page, you can replace the contents
			</li>
		</ul>
	</div>
</div>
-->

<h1 class="h1 px-5 pt-5">Chat Feature</h1>
<div class="p-5">
	<div class="grid grid-cols-[auto_1fr] gap-2 py-2">
		<Avatar src="https://i.pravatar.cc/?img=Person1" width="w-12" />
		<div class="card p-4 variant-soft rounded-tl-none space-y-2">
			<header class="flex justify-between items-center">
				<p class="font-bold">Artist 1</p>
				<small class="opacity-50">Yesterday @ 11:26</small>
			</header>
			<p>
				I love your art!
				Although one piece of advise I would give is to maybe focus more on the overall meaning of your art? Or maybe I'm just not your target audience.
			</p>
		</div>
	</div>

	<div class="grid grid-cols-[1fr_auto] gap-2 py-2">
		<div class="card p-4 rounded-tr-none space-y-2 variant-soft-primary">
			<header class="flex justify-between items-center">
				<p class="font-bold">Artist 2</p>
				<small class="opacity-50">Today @ 12:38</small>
			</header>
			<p>Hmm... I guess I never gave my art much thought. I always kinda just went with the flow, y'know. Not really knowing what comes next, that's what I vibe with.</p>
		</div>
		<Avatar src="https://i.pravatar.cc/?img=Person2" width="w-12" />
	</div>

	<div class="grid grid-cols-[auto_1fr] gap-2 py-2">
		<Avatar src="https://i.pravatar.cc/?img=Person1" width="w-12" />
		<div class="card p-4 variant-soft rounded-tl-none space-y-2">
			<header class="flex justify-between items-center">
				<p class="font-bold">Artist 1</p>
				<small class="opacity-50">Today @ 1:43</small>
			</header>
			<p>
				That's fair. Art is about freedom, after all. Although do give it a shot, thinking deeply while making art I mean. Who knows, maybe something brilliant can come out of it?
			</p>
		</div>
	</div>

	<div class="py-2">
		<div class="input-group input-group-divider grid-cols-[auto_1fr_auto] rounded-container-token">
			<button class="input-group-shim">+</button>
			<textarea
				class="bg-transparent border-0 ring-0"
				name="prompt"
				id="prompt"
				placeholder="Write a message..."
				rows="1"
			/>
			<button class="variant-filled-primary">Send</button>
		</div>
	</div>
</div>