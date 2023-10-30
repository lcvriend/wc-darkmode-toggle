# darkmode-toggle (web component)

`<darkmode-toggle>` is a web component that lets a user switch between light and dark mode:

* Super simple
* VanillaJS (no dependencies)
* Reacts to system preference
* Stores and loads set preference
* Dispatches a `color-scheme-change` event on change

## How to use
Load the `<darkmode-toggle>` web component and add it to your page:

```html
<darkmode-toggle></darkmode-toggle>
<script src="src/wc-darkmode-toggle.js"></script>
```

Listen for the `color-scheme-change` event and change your page accordingly. For example:

```javacript
document.addEventListener("color-scheme-change", event => {
    event.detail.scheme === "dark"
    ? document.body.classList.add("dark-theme")
    : document.body.classList.remove("dark-theme")
})
```
