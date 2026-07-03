# wana.yazi

Warm, bookish Gruvbox-leaning [yazi](https://github.com/sxyazi/yazi) flavors with
dark + light variants, generated from the canonical
[Wana](https://github.com/atalariq/wana) base24 palette.

This repo ships **two** flavors — `wana-dark` and `wana-light` (not `wana`).

## Install

```sh
ya pkg add atalariq/wana.yazi:wana-dark
ya pkg add atalariq/wana.yazi:wana-light
```

Then in `~/.config/yazi/theme.toml`:

```toml
[flavor]
dark  = "wana-dark"
light = "wana-light"
```

Restart yazi to apply (theme.toml is read at startup).

> **Gotcha:** yazi resolves a flavor by `<name>.yazi/`, so the flavor name must
> be `wana-dark` / `wana-light` — `dark = "wana"` looks for a nonexistent
> `wana.yazi/`.

## Manual / local install

Copy or symlink a flavor into `~/.config/yazi/flavors/` (symlink is handy when
hacking on the flavor itself):

```sh
ln -s /path/to/wana-dark.yazi  ~/.config/yazi/flavors/wana-dark.yazi
ln -s /path/to/wana-light.yazi ~/.config/yazi/flavors/wana-light.yazi
```

> Generated — do not hand-edit the flavor files. Source of truth: `schemes/` in
> [atalariq/wana](https://github.com/atalariq/wana).
