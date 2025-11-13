# WP Flex Reverse Toggle

This little package exports a single function, `addFlexReverseToggle` that wires up an extra toggle component to reverse the flex direction of certain core blocks.

**Note:** The source file is currently only built in Typescript. Be sure to import it into a Typescript file!

## Blocks

1. `core/group`
2. `core/columns`

## Getting Started & Sample Usage

1. Import the `addFlexReverseToggle` function into your working file
2. Enqueue your working file into the WP Admin with the `enqueue_block_editor_assets` hook

```ts
// the rest of your JS/TS file to edit the Block Editor....

function alterBlocks(): void {
	// namespace can be anything, and should be unique to your plugin/theme
	const namespace = 'cno-starter-theme';
	addFlexReverseToggle(namespace);
}
alterBlocks();

// the rest of your JS/TS file to edit the Block Editor....
```

## Changelog

### v1.1.2 - [November 13, 2025]

- Fixed: Hooks return new objects appropriately instead of mutating objects
- Chore: Update packages

### v1.1.1 - [July 2, 2025]

- Fix: Build files are included in npm registry
- Fix: TS errors/warnings are ignored
- Fix: add missing dev dependencies

### v1.1.0 - [July 2, 2025]

- Update build to allow proper imports with WP projects

### v1.0.1 - [July 2, 2025]

- Update dependencies

### v1.0.0 - [July 2, 2025]

- First build! This component works with `core/group` and `core/columns` blocks.
