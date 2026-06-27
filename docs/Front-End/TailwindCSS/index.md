# Tailwind CSS 101

Tailwind CSS is a utility-first [CSS](../CSS/index.md) framework, which gives the developer access to a collection of classes that can be composed to build designs directly in [HTML](../HTML/index.md).

## How to install

To install Tailwind, we should use the [NPM](../../NPM/index.md) packet manager in our project,

```bash
npm install tailwindcss @tailwindcss/cli
```

## How to use

As said, Tailwind builds for us the [CSS](../CSS/index.md) for the project, given an instruction set of Tailwind's commands. For example this command to import `tailwindcss`,

```css
@import "tailwindcss";
```

Then, to create the [CSS](../CSS/index.md) of our project from the Tailwind's , we need to use the following [npx](../../NPM/NPX.md) command,

```bash
npx @tailwindcss/cli -i <tailwind-instructions-file> -o <css-file>
```

it's good practice to use an [npm script](../../NPM/package.json.md#npm-scripts) for this operation.

Now to actually use the [CSS](../CSS/index.md) provided by Tailwind, you can use the following syntax,

```html
<tag class="tailwind-class-1 tailwind-class-2 tailwind-class-3 ...">
	...
</tag>
```

those classes can be found by searching the docs at [the official site](https://tailwindcss.com/docs/installation/tailwind-cli), or in [this cheat sheet](https://www.creative-tim.com/twcomponents/cheatsheet).

## Integration with IDE

To leverage the Tailwind framework to it's maximum it's expected of you to use the plugin for Tailwind in visual studio code, [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss).
