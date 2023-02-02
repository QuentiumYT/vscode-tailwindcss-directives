# Tailwindcss directives

## Description

This VSCode extension adds support for Tailwindcss directives. By default, @apply, @tailwind, @screen, etc... are not recognized by the CSS language server. This extension include a custom data file that loads them inside your CSS & SCSS files. It will also show a description and a link to the documentation when you hover over a directive.

⚠️ Support Tailwind v3 and also v2 (included alongside v3)

Documentation about custom data can be found here: https://github.com/microsoft/vscode-css-languageservice/blob/main/docs/customData.md

Based on rules from this issue: https://github.com/tailwindlabs/tailwindcss-intellisense/issues/69

## Installation

The easiest and recommended way is simply to install this extension from the VSCode marketplace.

You can also copy the `tailwind.css-data.json` file into your project root and add the following to your `settings.json` file:

```json
"css.customData": [
  "./tailwind.css-data.json"
]
```

(you can also put it inside a `.vscode` folder and set the path to `./.vscode/tailwind.css-data.json`)

The last option is to run this extension in the **Debug** tab and select the **Launch Extension** configuration. This will open a new VSCode window with the extension installed.
