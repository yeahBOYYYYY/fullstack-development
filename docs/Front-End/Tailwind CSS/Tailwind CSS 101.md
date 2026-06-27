# Tailwind CSS 101

Tailwind CSS is a utillity-first [[CSS 101|CSS]] framework, which gives the developer access to a collection of classes that can be composed to build designs directly in [[HTML 101|HTML]].

## How to install

To install Tailwind, we should use the [[NPM 101|NPM]] packet manager in our project,

```bash
npm install tailwindcss @tailwindcss/cli
```

## How to use

As said, Tailwind builds for us the [[CSS 101|CSS]] for the project, given an instruction set of Tailwind's commands. For example this command to import `tailwindcss`,

```css
@import "tailwindcss";
```

Then, to create the [[CSS 101|CSS]] of our project from the Tailwind's , we need to use the following [[NPX|npx]] command,

```bash
npx @tailwindcss/cli -i <tailwind-instructions-file> -o <css-file>
```

it's good practice to use an [[package.json file#npm scripts|npm script]] for this operation.

Now to actually use the [[CSS 101|CSS]] provided by Tailwind, you can use the following syntax,

```html
<tag class="tailwind-class-1 tailwind-class-2 tailwind-class-3 ...">
	...
</tag>
```

those classes can be found by searching the docs at [the official site](https://tailwindcss.com/docs/installation/tailwind-cli), or in [this cheat sheet](https://www.creative-tim.com/twcomponents/cheatsheet).
## Integration with IDE

To leverage the Tailwind framework to it's maximum it's expected of you to use the plugin for Tailwind in visual studio code, [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss).