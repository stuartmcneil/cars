# Cars — Owners Workshop Manual

Every car I have owned, written up in the style of a workshop manual: a chapter per car, oldest first, each with a line drawing, factory specifications and owner's notes.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole page — layout, callouts and text. The only external dependency is Google Fonts; without them it falls back to system fonts. |
| `art/*.png` | The ink-traced car illustrations (transparent PNGs), one per car, referenced from `index.html` as `art/<name>.png`. Upload this folder alongside `index.html`. |
| `photos/` | Source photographs used for the tracings. Not needed on GitHub. |

## Put it on GitHub

1. On github.com, **New repository** → name it `cars` → **Public** → Create.
2. **Add file → Upload files**, drag in `index.html`, the whole `art` folder and this `README.md`, commit.
3. **Settings → Pages** → Source: *Deploy from a branch*, Branch: `main`, folder `/ (root)` → Save.
4. After a minute it is live at `https://stuartmcneil.github.io/cars/`.

## Link it from the windowsill

In `Web/index.html`, the toy-car entry currently has no link. Add one:

```js
{ id:'cars', object:'Red toy car', label:'Cars',
  href:'https://stuartmcneil.github.io/cars/',
  ...
```

## Editing

Each car is a `<section class="page" id="cN">`. To add a car, copy the last chapter, change the number, the heading, the plate, the spec table and the notes. Anything still marked `tbc` (class `tbc`, shown in brown italics) is a gap to fill in.
