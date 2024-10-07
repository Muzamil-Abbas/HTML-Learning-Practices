# HTML Notes

## Basic Structure

- **DOCTYPE**: Declares the document type and version of HTML (e.g., `<!DOCTYPE html>` for HTML5).
- **html**: Root element of an HTML page, encapsulating all other elements.
- **head**: Contains metadata and links to external resources.
  - **title**: Title of the document displayed in the browser tab.
  - **meta**: Provides metadata such as character set (`<meta charset="UTF-8">`), viewport settings (`<meta name="viewport" content="width=device-width, initial-scale=1.0">`), and description.
  - **link**: Used to link external stylesheets (`<link rel="stylesheet" href="styles.css">`).
  - **script**: Links to external JavaScript files, typically placed before the closing `</body>` tag for better performance.

## Body Content

- **body**: Main content of the HTML document.
  - **h1-h6**: Header tags used for titles and subtitles, where `h1` is the most important and `h6` the least.
  - **p**: Paragraphs of text, automatically adding space above and below.
  - **a**: Hyperlinks to other pages or sections (`<a href="https://example.com">Link</a>`).
  - **img**: Images with attributes for source (`src`), alt text for accessibility (`alt`), width, and height.
  - **ul/ol**: Unordered (bulleted) or ordered (numbered) lists, respectively.
  - **li**: List items within `ul` or `ol`.
  - **div**: Block-level container for grouping elements, useful for layout purposes.
  - **span**: Inline container for styling a portion of text, often used for applying styles without breaking flow.
  - **blockquote**: Used to indicate a section quoted from another source.

## Forms and Input

- **form**: Container for form elements, using the `action` attribute to specify the destination for form data.
  - **input**: Various input types (`text`, `password`, `checkbox`, `radio`, `file`, `submit`, etc.) with the `type` attribute.
  - **label**: Labels for input elements, linked via the `for` attribute.
  - **textarea**: Multi-line text input, often for comments or descriptions.
  - **button**: Clickable button for form submission or custom actions (`<button type="submit">Submit</button>`).
  - **select**: Dropdown list, with `option` elements as choices.
  - **fieldset**: Groups related elements in a form, often with a legend.

## Semantic HTML

- **header**: Represents introductory content or a group of navigational links.
- **nav**: Contains navigation links, enhancing site structure for search engines and accessibility.
- **main**: Main content area of the document, unique to the document.
- **section**: Represents a thematic grouping of content, typically with a heading.
- **article**: Self-contained content that could be distributed independently, such as blog posts or news articles.
- **aside**: Content tangentially related to the main content, such as sidebars or pull quotes.
- **footer**: Footer for the document or section, often containing copyright information, links, or contact details.

## Accessibility

- Use **alt** attributes for images for screen readers, providing meaningful descriptions.
- Use semantic HTML for better accessibility and SEO, helping assistive technologies understand content structure.
- Ensure forms have associated labels for input elements, improving usability for screen reader users.
- Consider color contrast for readability, ensuring text is legible against backgrounds.
- Use ARIA roles and properties to enhance accessibility where semantic HTML is insufficient.

## Responsive Design

- Use **meta viewport** tag for responsive design on mobile devices: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`.
- Utilize CSS media queries to adjust layout for different screen sizes, enhancing user experience across devices.
- Use relative units like percentages (`%`) and viewport units (`vw`, `vh`) for fluid layouts.
- Implement mobile-first design by writing styles for smaller screens first, then enhancing for larger devices.

## Multimedia

- **audio**: Embeds sound content. Supports formats like MP3, WAV, and Ogg.
  - Attributes: `controls`, `autoplay`, `loop`, `muted`, and `preload`.
- **video**: Embeds video content with support for formats like MP4, WebM, and Ogg.
  - Attributes: `controls`, `autoplay`, `loop`, `muted`, `poster`, and `preload`.
  - **track**: Used within video to provide text tracks for subtitles or captions.

## Meta Tags for SEO

- **description**: Provides a summary of the page content for search engines (e.g., `<meta name="description" content="Your page description here.">`).
- **keywords**: Although less relevant now, can still be used to specify target keywords.
- **robots**: Directs search engines on how to index a page (e.g., `index`, `noindex`).
- **canonical**: Prevents duplicate content issues by specifying the preferred version of a URL (`<link rel="canonical" href="https://example.com/preferred-url/">`).

## Best Practices

- Keep HTML clean and well-indented for readability.
- Validate HTML to ensure it meets web standards (use tools like W3C Validator).
- Use comments (`<!-- comment -->`) to explain sections of your HTML for future reference.
- Minimize the use of inline styles; prefer external CSS for better separation of concerns.
- Optimize images for web use to enhance loading times.
- Use lowercase for all HTML tags and attributes for consistency and adherence to best practices.

## Common HTML Entities

- Use HTML entities for special characters:
  - `&nbsp;` for non-breaking space.
  - `&lt;` for less than (`<`).
  - `&gt;` for greater than (`>`).
  - `&amp;` for ampersand (`&`).
  - `&quot;` for quotation mark (`"`).
  - `&copy;` for copyright symbol (`©`).
  - `&reg;` for registered trademark symbol (`®`).
  - `&trade;` for trademark symbol (`™`).

## HTML5 Features

- **Canvas**: Allows for dynamic, scriptable rendering of 2D shapes and bitmap images using JavaScript.
  - Usage involves creating a `<canvas>` element and drawing on it via the Canvas API.
- **Local Storage**: Provides a way to store data locally within the user's browser using key/value pairs, persisting even after the browser is closed.
- **Geolocation**: Enables access to the user's location via the `navigator.geolocation` API, allowing location-based features.
- **Web Workers**: Allows running scripts in background threads, improving performance by offloading tasks from the main thread.

## Advanced Topics

- **Custom Data Attributes**: Use `data-*` attributes to store custom data on elements for JavaScript manipulation (e.g., `<div data-user-id="123">`).
- **Progressive Enhancement**: Build a basic functional experience that works across all browsers and enhance it for more capable ones.
- **Graceful Degradation**: Start with a full-featured experience and ensure that core functionalities work even in older browsers.

## Resources

- [Mozilla Developer Network (MDN) Web Docs](https://developer.mozilla.org/)
- [HTML Living Standard](https://html.spec.whatwg.org/multipage/)
- [Can I use](https://caniuse.com/) - A resource to check browser support for HTML features.
