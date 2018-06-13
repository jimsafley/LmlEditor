# LML Editor

Turn any textarea into a lightweight markup language (LML) editor.

```html
<script type="text/javascript" src="/js/vendor/LmlEditor.js"></script>

<div id="lml-editor-buttons"></div>
<textarea id="lml-editor-textarea"></textarea>

<script>
// Initialize the LML editor.
var lmlEditor = new LmlEditor(
    document.getElementById('lml-editor-textarea'),
    document.getElementById('lml-editor-buttons')
);
// Add the bundled set of MediaWiki buttons.
lmlEditor.addMediawikiButtons();
// Add an individual MediaWiki button.
lmlEditor.addButton('wikitext-editor-button-signature', 'Signature', "", "-- ~~~~\n");
</script>
```

## Translations

To translate button titles, add a "data-lml-editor-translations" data attribute to the button container containing a JSON object where keys are original strings and values are translated strings.

```html
<div id="lml-editor-buttons" data-lml-editor-translations="{&quot;Underline&quot;:&quot;Subrayar&quot;}"></div>
```
