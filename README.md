# opencode-centered-layout

Centers the [OpenCode](https://opencode.ai) TUI session pane on wide terminals
instead of stretching it full-width. Toggle any time with `/center`.

Depends on OpenCode internals (the `session-pane` renderable). If an OpenCode
update breaks it, the plugin warns once and leaves the default layout unchanged —
never a broken UI.

## Install

TUI-only plugins load from `cli.json` (not `opencode.json`):

```jsonc
// ~/.config/opencode/cli.json
{
  "plugins": ["opencode-centered-layout@git+https://github.com/joseph280996/opencode-centered-layout.git"]
}
```

| Keybind/UI | Action |
|---|---|
| `/center` or command palette → "Toggle centered layout" | on/off (persisted via plugin storage) |

Tested on OpenCode v2.2.2.

## License

MIT
