# shadcn-svelte Safari scrolling reproduction

This is a reproduction of weird scrolling behaviors with some shadcn-svelte components in iOS Safari.

## Steps to reproduce

1. Clone this repo
2. Run `pnpm install`
3. Run `pnpm dev --host` or build first with `pnpm build` and then run `pnpm start --host`
4. Open the app in iOS (or iPadOS) Safari
5. Scroll a bit down
6. Tap on the "Open DropdownMenu" button
7. Tap anywhere outside the dropdown menu to close it
8. See the weird scrolling behavior

## Expected behavior

1. Follow the steps 1 to 5 above
2. Tap on the "Open Popover" button
3. Tap anywhere outside the popover to close it
4. No weird scrolling behavior