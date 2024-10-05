<script lang="ts">
	import { Button } from "$lib/components/ui/button";
	import { Input } from "$lib/components/ui/input";
	import { Separator } from "$lib/components/ui/separator";
	import { Mail } from "lucide-svelte";

</script>

<div class="grid grid-cols-2 h-full place-items-center">
    <aside class="max-w-2xl">
        <img src="/assets/images/logistics.svg" alt="logistics">
    </aside>
    <main class="flex flex-col gap-16 px-4 w-full max-w-md mx-auto">
        <div class="text-center">

            <h1 class="text-3xl">Crează un cont</h1>
            <p class="text-sm text-muted-foreground">Introdu adresa de email pentru a crea un contdawd</p>
        </div>

        <div class="flex flex-col gap-2">
            <div class="relative">
                <Input placeholder="email@example.com" class="pl-10" />
                <Mail class="absolute top-1/2 -translate-y-1/2 left-2 text-primary" />
            </div>
            <Button>Logare cu email</Button>
        </div>

        <div class="flex items-center justify-center relative">
            <Separator />
            <span class="absolute bg-background px-4"> SAU CONTINUĂ CU </span>
        </div>

        <div class="flex flex-col gap-2">

            <Button variant="outline">Google</Button>
            <Button variant="outline">Github</Button>
        </div>

        <p class="text-sm text-center">By clicking continue, you agree to our Terms of Service and Privacy Policy.</p>
    </main>
</div>