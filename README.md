### [ ` g a m e w o r k s ` ](https://github.com/scrollingbot/gameworks)
<p>u i &nbsp f r a m e w o r k </p>


**g a m e w o r k s** is a ui component library for [`s v e l t e k i t`](https://kit.svelte.dev/).


<p>g e t &nbsp  s t a r t e d :</p>

```bash
npm i sidemoney
```

To use the layout components, create a css file `src/app.css`:

```css
body, html {
    height: 100%;
    width: 100%;
    margin: 0;
  }
```

and implement it from your main `+layout.svelte` file like so:

```javascript
<script>
    import '../app.css';
</script>

```

To use the animated components, the `vite-plugin-wasm` and `vite-plugin-top-level-await` plugins are required. Install these with: 

```bash
npm i vite-plugin-wasm
npm i vite-plugin-top-level-await
```

And modify your `vite.config.js` file as such:

```javascript
import { sveltekit } from '@sveltejs/kit/vite';
import { defineConfig } from 'vite';
import wasm from "vite-plugin-wasm";
import topLevelAwait from "vite-plugin-top-level-await";


export default defineConfig({
  plugins: [sveltekit(), topLevelAwait(), wasm()]
});
```
