<script lang="ts">
	import * as DropdownMenu from '$lib/components/ui/dropdown-menu';
	import * as Popover from '$lib/components/ui/popover';

	const colors = ['red', 'yellow', 'green', 'blue', 'indigo', 'purple', 'pink'];

	const allColors = [...colors, ...colors];
</script>

{#each allColors as color, i (i)}
	<div class="h-40" style="background-color: {color}" />
{/each}

<div
	class="fixed text-white bottom-0 py-4 flex justify-center items-center gap-10 left-0 right-0 bg-background"
>
	<DropdownMenu.Root>
		<DropdownMenu.Trigger class="px-4 py-2 rounded-lg bg-neutral-800">
			Open DropdownMenu
		</DropdownMenu.Trigger>
		<DropdownMenu.Content>
			<DropdownMenu.Group>
				<DropdownMenu.Label>My Account</DropdownMenu.Label>
				<DropdownMenu.Separator />
				<DropdownMenu.Item>Profile</DropdownMenu.Item>
				<DropdownMenu.Item>Billing</DropdownMenu.Item>
				<DropdownMenu.Item>Team</DropdownMenu.Item>
				<DropdownMenu.Item>Subscription</DropdownMenu.Item>
			</DropdownMenu.Group>
		</DropdownMenu.Content>
	</DropdownMenu.Root>

	<Popover.Root>
		<Popover.Trigger class="px-4 py-2 rounded-lg bg-neutral-800">Open Popover</Popover.Trigger>
		<Popover.Content>Place content for the popover here.</Popover.Content>
	</Popover.Root>
</div>
