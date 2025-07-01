# Interactive FAQ System

A smart, searchable FAQ component with voting and analytics features.

## Features

- 🔍 Fuzzy search with Fuse.js
- 🏷️ Category filtering
- 👍 Helpfulness voting
- 📊 View count tracking
- 📱 Mobile responsive
- ♿ Accessible (WCAG 2.1 AA)

## Data Structure

FAQs are stored in JSON format:

```json
{
  "id": "unique-id",
  "question": "Question text",
  "answer": "Answer text (supports markdown)",
  "category": "Category name",
  "tags": ["tag1", "tag2"],
  "views": 0,
  "helpful": 0,
  "notHelpful": 0
}
```

## Usage

```tsx
import FAQ from './apps/faq/FAQ';

<FAQ />
```

## WordPress Integration

Embed in WordPress using:

```html
<div id="evomics-faq"></div>
<script src="https://shandley.github.io/evomics-web/faq-embed.js"></script>
```