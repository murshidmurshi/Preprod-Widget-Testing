# Intentick Preprod Widget Testing

Testbed and dynamic script loader for the Intentick Preprod Widget with customizable Collect ID management.

## Features

- **Embedded Widget Script**:
  ```html
  <script
    src="https://preprod.intentick.com/intentick_widget.js"
    data-collect-id="Intentick_widget_r7v9swxw"
    async
  ></script>
  ```
- **Default Collect ID**: `Intentick_widget_r7v9swxw`
- **Dynamic ID Switching**: A built-in button in the top-left triggers a native browser `prompt()` to input a custom Collect ID, displays an `alert()` confirmation, and reloads the page with persistent `localStorage` and URL parameters (`?collect_id=...`).
- **Interactive Test Sandbox**: Includes high-intent CTA click targets, sample lead generation form, feature interaction cards, and a real-time event console.

## Getting Started

Open `index.html` directly in your browser, or start a local server:

```bash
# Using Python
python3 -m http.server 8080

# Using Node (npx)
npx serve .
```

Visit `http://localhost:8080` in your web browser.
