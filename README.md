# Tokyo Night Dark for Limine

Tokyo Night Dark theme for the [Limine](https://limine-bootloader.org/)
bootloader.

## Files

- [`themes/tokyonight-dark.conf`](./themes/tokyonight-dark.conf): ready-to-use
  Limine theme snippet
- [`limine.tera`](./limine.tera): source template used to generate the theme

## Palette

- Background: `#1a1b26`
- Foreground: `#c0caf5`
- Bright background: `#414868`
- ANSI accents: `#f7768e`, `#9ece6a`, `#e0af68`, `#7aa2f7`, `#bb9af7`,
  `#7dcfff`

## Usage

1. Open your Limine configuration file, usually `/boot/limine.conf` or
   `/boot/efi/limine.conf`.
2. Paste the contents of
   [`themes/tokyonight-dark.conf`](./themes/tokyonight-dark.conf) at the top of
   the file.
3. Save the config and reboot.

## Regenerating

If you change [`limine.tera`](./limine.tera), regenerate the output with:

```sh
just build
```

This runs `whiskers limine.tera` and rewrites
[`themes/tokyonight-dark.conf`](./themes/tokyonight-dark.conf).

## FAQ

- Q: How do I hide the Limine title text?
  A: Add `interface_branding:` with an empty value in your Limine config.

- Q: Where are the other Limine configuration options documented?
  A: See
  [limine/CONFIG.md](https://github.com/limine-bootloader/limine/blob/v8.x/CONFIG.md).

## Credits

- Original Limine theme structure based on work by
  [mekb](https://github.com/mekb-turtle)
