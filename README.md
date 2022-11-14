# vscode-svelte-pluskit-snippets

<a href="https://marketplace.visualstudio.com/items?itemName=garlandcrow.vscode-svelte-pluskit-snippets" target="__blank"><img src="https://img.shields.io/visual-studio-marketplace/v/garlandcrow.vscode-svelte-pluskit-snippets.svg?color=eee&amp;label=VS%20Code%20Marketplace&logo=visual-studio-code" alt="Visual Studio Marketplace Version" /></a>

Adds starter snippets for:

- +page.ts
- +page.server.ts
- +page.svelte
- +layout.ts
- +layout.server.ts
- +layout.svelte
- +server.ts
- +error.svelte

with the types imported and the common exported things, for example:

`+page.ts`

```ts
import { error, invalid, redirect } from "@sveltejs/kit";
import type { PageServerLoad, Actions } from "./$types";

export const load: PageServerLoad = async function (event) {
  return {};
};

export const actions: Actions = {
  default: async (event) => {
    return {};
  },
};
```

OK, and here's the really nice part, it adds a keyboard shortcut `cmd+k n` that automatically inserts the snippet that corresponds to the file you are in (make sure its blank). So you don't have to remember all the boilerplate for each file just create the file and `cmd+k n` in whatever file type of +kit.

File an issue [here](https://github.com/garlandcrow/vscode-svelte-pluskit-snippets/issues) if there are more templates to be added or more things you think should be in the templates by default.

## Sponsors

<p align="center">
  <a href="https://cdn.jsdelivr.net/gh/garlandcrow/static/sponsors.svg">
    <img src='https://cdn.jsdelivr.net/gh/garlandcrow/static/sponsors.png'/>
  </a>
</p>

## License

[MIT](./LICENSE) License © 2022 [Garland Crow](https://github.com/garlandcrow)
