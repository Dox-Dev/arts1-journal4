<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->
<script lang="ts">
	import Hero from "$lib/Hero.svelte";
	import { Avatar } from "@skeletonlabs/skeleton";
	import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
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


<h1 class="h1 px-5 pt-5">Art Gallery</h1>
<p class="px-5 pt-5">
	Note that these images (as well as the card components themselves) were taken from the <a href="https://www.skeleton.dev/elements/image-layouts" target="_blank" class="underline">SkeletonUI</a> website,
	which directly attributes these image layouts to <a href="https://flowbite.com" target="_blank" class="underline">Flowbite</a>.
</p>
<div class="p-5">
	<section class="grid grid-cols-2 md:grid-cols-4 gap-2">
		<div class="grid gap-4">
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1617296538902-887900d9b592?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzExMDB8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" />
			</div>
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1597077962467-be16edcc6a43?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY2MzZ8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1591775161903-497839a443c1?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY3MzR8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
		</div>
		<div class="grid gap-4">
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1617296539691-67feaadf389e?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY3NjF8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1542835435-4fa357baa00b?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY3NzN8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1553184570-557b84a3a308?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY2NTF8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
		</div>
		<div class="grid gap-4">
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1603855873822-0931a843ee3a?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY3ODJ8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1509130446053-899ae7358ce6?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY2NjF8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1508931133503-b1944a4ecdd5?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY3OTV8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
		</div>
		<div class="grid gap-4">
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1633053663400-655b31fb88ac?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY4MDV8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1578170222009-c7893aa20afd?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY4MTZ8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
			<div>
				<img class="h-auto max-w-full rounded-lg card-hover hover:opacity-50" src="https://images.unsplash.com/photo-1610220941077-1ec123e7c043?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY4NjV8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max" alt="" />
			</div>
		</div>
	</section>
</div>




<h1 class="h1 px-5 pt-5">Art Tutorials</h1>
<!--
<p class="px-5 pt-5">Note that these images (as well as the card components themselves) were taken from the <a href="https://www.skeleton.dev/elements/image-layouts" target="_blank" class="underline">SkeletonUI</a> website.</p>
-->
<div class="p-5">
	<Accordion>
		<AccordionItem>
			<svelte:fragment slot="lead"><i class="fa-solid fa-spray-can"></i></svelte:fragment>
			<svelte:fragment slot="summary">Spray Painting/Graffiti Art</svelte:fragment>
			<svelte:fragment slot="content">This is where guides for spray painting will be placed in.</svelte:fragment>
		</AccordionItem>
		<AccordionItem>
			<svelte:fragment slot="lead"><i class="fa-solid fa-palette"></i></svelte:fragment>
			<svelte:fragment slot="summary">Traditional Painting</svelte:fragment>
			<svelte:fragment slot="content">This is where guides for traditional painting will be placed in.</svelte:fragment>
		</AccordionItem>
		<AccordionItem>
			<svelte:fragment slot="lead"><i class="fa-solid fa-person"></i></svelte:fragment>
			<svelte:fragment slot="summary">Sculpting</svelte:fragment>
			<svelte:fragment slot="content">This is where guides for sculpting will be placed in.</svelte:fragment>
		</AccordionItem>
		<AccordionItem>
			<svelte:fragment slot="lead"><i class="fa-solid fa-tablet"></i></svelte:fragment>
			<svelte:fragment slot="summary">Digital Art</svelte:fragment>
			<svelte:fragment slot="content">This is where guides for digital art will be placed in.</svelte:fragment>
		</AccordionItem>
		<AccordionItem>
			<svelte:fragment slot="lead"><i class="fa-solid fa-camera"></i></svelte:fragment>
			<svelte:fragment slot="summary">Photography</svelte:fragment>
			<svelte:fragment slot="content">This is where guides for photography will be placed in.</svelte:fragment>
		</AccordionItem>
		<AccordionItem>
			<svelte:fragment slot="lead"><i class="fa-solid fa-video"></i></svelte:fragment>
			<svelte:fragment slot="summary">Videography/Film</svelte:fragment>
			<svelte:fragment slot="content">This is where guides for film will be placed in.</svelte:fragment>
		</AccordionItem>
		<!-- ... -->
	</Accordion>
</div>