# mk2mk

A simple way to render markdown as PDF without installing local tooling.

## Usage

1. Visit [https://davekinkead.github.io/mk2mk/](https://davekinkead.github.io/mk2mk/)
2. Type or paste markdown
3. Select a theme from the dropdown
4. Click "Export PDF" to print/save as PDF

## Supported Markdown Syntax

| Syntax | Example |
|--------|---------|
| Headings | `# H1` through `###### H6` |
| Bold | `**text**` or `__text__` |
| Italic | `*text*` or `_text_` |
| Links | `[text](url)` |
| Images | `![alt](url)` |
| Inline code | `` `code` `` |
| Code blocks | ` ``` ` fences |
| Blockquotes | `> quote` |
| Unordered lists | `-`, `*`, `+` |
| Ordered lists | `1.` |
| Horizontal rules | `---`, `***`, `___` |

## Adding Custom Themes

1. Create a new CSS file in `themes/community/` (e.g., `solarized.css`)
2. Define the CSS variables (copy from an existing theme as a template)
3. Add the theme to the dropdown in `index.html`
4. Submit a pull request

### Theme Template

```css
:root {
  --app-bg: #...;
  --app-fg: #...;
  --header-bg: #...;
  --border-color: #...;
  --logo-color: #...;
  --button-bg: #...;
  --button-fg: #...;
  --button-hover-bg: #...;
  --editor-bg: #...;
  --editor-fg: #...;
  --editor-caret: #...;
  --line-num-bg: #...;
  --line-num-fg: #...;
  --placeholder-fg: #...;

  --md-heading: #...;
  --md-bold: #...;
  --md-italic: #...;
  --md-link: #...;
  --md-url: #...;
  --md-code: #...;
  --md-code-bg: #...;
  --md-code-block: #...;
  --md-fence: #...;
  --md-quote: #...;
  --md-list: #...;
  --md-hr: #...;
  --md-image: #...;
}
```

## Browser Support

Works in modern browsers:
- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

### Print Notes

For best PDF results:
- Chrome/Safari/Edge: Background colors print automatically
- Firefox: Enable `print.print_bgcolor` in `about:config` if backgrounds don't print

## License

MIT
