# MkDocs Setup

## Python Requirements
Install the following packages via pip.

```
markdown-wavedrom
mkdocs
mkdocs-material
```

## mkdocs.yaml Example for this Page

```yaml
site_name: Markdown WaveDrom Example

theme:
  name: material

markdown_extensions:
  - admonition
  - markdown_wavedrom
  - pymdownx.details
  - pymdownx.superfences

extra_javascript:
  - https://cdnjs.cloudflare.com/ajax/libs/wavedrom/2.6.8/wavedrom.min.js
  - https://cdnjs.cloudflare.com/ajax/libs/wavedrom/2.6.8/skins/default.js
  - js/wavedrom_loader.js

```

## js/wavedrom_loader.js Content
```js
window.addEventListener("load", function () {
  WaveDrom.ProcessAll();
});

```
