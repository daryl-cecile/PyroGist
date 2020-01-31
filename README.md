# PyroGist
 
A small library to embed files from **public GitHub repos**. This library is ideal for people looking to embed files from GitHub into their website.

![](info/Screenshot%202020-01-31%20at%2018.40.50.png)

---

### Usasge

To start using the library, first include the script and style in your webpage (preferably in the `<head>` tag). **Note:** make sure you change the path to point to the resources from your folder.

```html
<link rel="stylesheet" href="src/PyroGist.css">
<script src="src/PyroGist.js"></script>
```

Once you have the above tags, you can start by calling `PyroGist()` method, passing in the selector of the container you would like to use, as well as the options:

```javascript
PyroGist("#preview",{
    url: "https://github.com/daryl-cecile/Slosh/blob/master/library/defaultStyle.css",
    theme: "normal",
    autoFit: true,
    highlight: true
});
```

In the example above, `theme`, `autoFit` and `highlight` options are used. However, these are optional.

---

#### Options
- `theme`: string [optional]
    - accepts _dark_, _ultraDark_, _match_, and _normal_. 
    - `Match` will try to match the rest of your page.

- `autoFit`: boolean [optional]
    - accepts `true` or `false`.
    - `true` will cause the container to resize reasonably if content is too long

- `highlight`:boolean [optional]
    - accepts `true` or `false`
    - Uses highlight.js to perform syntax highlighting.
    - Will only work if highlight.js has been included into the webpage 

---

#### Try it out
You can try this out for yourself by cloning this repo and opening the `index.html` file in a web browser.

---

### Notes:
This project makes use of [JetBrainsMono](https://github.com/JetBrains/JetBrainsMono), an open source font by JetBrains.