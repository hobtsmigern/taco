# 🌮 Which taco are you?

A tiny, cute personality quiz. Answer 9 questions and find out which of 12 tacos matches your personality, from the main-character energy of **Al Pastor** to the dreamy chaos of the **Ice Cream** taco.

Everything lives in one file (`index.html`): no build step, no dependencies, no framework.

## Features

- 12 tacos, each with its own hand-drawn (well, code-drawn) SVG illustration and personality
- A flavor profile on 4 axes: spice, energy, social and adventure
- Runner-up taco and "best taco buddy" for every result
- Shareable result links (e.g. `.../#birria`) and native sharing on phones
- A gallery of all 12 tacos
- Works on mobile, supports dark mode, keyboard shortcuts (1–4) and reduced motion

## Host it on GitHub Pages

1. Create a new public repository on GitHub, for example `taco-quiz`.
2. Upload `index.html` and `README.md` to the root of the repository (Add file → Upload files).
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
5. After a minute or two your quiz is live at `https://YOUR-USERNAME.github.io/taco-quiz/`.

## Make it your own

All the content sits at the top of the `<script>` in `index.html`:

- `QUESTIONS`: each answer has an emoji, a label and a 4-number nudge `[spice, energy, social, adventure]`, each from -1 to 1.
- `TACOS`: each taco has a name, description, superpower, buddy, flavor profile (`vec`) and an `art` recipe (shell type, filling colors, toppings, face).
- `BALANCE`: small offsets that keep every taco roughly equally likely. If you add tacos or change questions, some results may become rarer; nudge the offset up to make a taco rarer or down to make it more common.

Available art options:

- Shells: `corn`, `flour`, `hard`, `blue`, `red`, `waffle`
- Faces: `happy`, `grin`, `wink`, `sleepy`, `dreamy`
- Toppings: `pineapple`, `onion`, `cilantro`, `cabbage`, `purple`, `cheese`, `tomato`, `kimchi`, `sesame`, `avocado`, `queso`, `potato`, `scallion`, `jalapeno`, `sprinkle`
- Extras: `lime: true`, `waves: ["crema"]` or `["choco"]`, `under: ["lettuce"]`

## License

MIT. Go make more tacos.
