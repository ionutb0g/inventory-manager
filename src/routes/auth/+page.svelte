<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Input } from '$lib/components/ui/input';
	import { Separator } from '$lib/components/ui/separator';
	import { Mail } from 'lucide-svelte';
</script>

<div class="grid h-full grid-cols-2 place-items-center">
	<aside class="max-w-2xl">
		<img src="/assets/images/logistics.svg" alt="logistics" />
	</aside>
	<main class="mx-auto flex w-full max-w-md flex-col gap-16 px-4">
		<div class="text-center">
			<h1 class="text-3xl">Creează un cont</h1>
			<p class="text-sm text-muted-foreground">Introdu adresa de email pentru a crea un cont</p>
		</div>

		<div class="flex flex-col gap-2">
			<div class="relative">
				<Input placeholder="email@example.com" class="pl-10" />
				<Mail class="absolute left-2 top-1/2 -translate-y-1/2 text-primary" />
			</div>
			<Button class="text-md font-extrabold">Logare cu email</Button>
		</div>

		<div class="relative flex items-center justify-center">
			<Separator />
			<span class="absolute bg-background px-4"> SAU CONTINUĂ CU </span>
		</div>

		<div class="flex flex-col gap-2">
			<Button variant="outline" class="text-md gap-4 font-extrabold">
				<img src="/assets/icons/google.webp" alt="google logo" class="h-full" />
				<span>Google</span>
			</Button>
			<Button variant="outline" class="text-md gap-4 font-extrabold">
				<img src="/assets/icons/github.webp" alt="google logo" class="h-full dark:invert" />
				<span>Github</span>
			</Button>
		</div>

		<!-- TODO: to create terms of service  -->
		<!-- TODO: to create privacy policy  -->
		<p class="text-center text-sm">
			<span> Prin crearea unui cont, sunteți de acord cu </span>
			<a href="/auth" class="text-primary"> Termenii Serviciului </a>
			<span> și </span>
			<a href="/auth" class="text-primary"> Politica de Confidențialitate </a>
			<span> . </span>
		</p>
	</main>
</div>
