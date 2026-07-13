# Component: Button

## Purpose
Creates a clickable button, typically used for links or calls to action.

## When to Use
* Linking to other pages on your site (e.g., "Learn More", "Contact Us").
* Linking to external websites.
* Highlighting the main action within a `CallToAction` component.
* Creating eye-catching call-to-action elements in your content.

## How to Use (Options / Props)

You add options (called "props") inside the opening tag `<Button ... >`. The text you want *inside* the button goes between the opening `<Button>` and closing `</Button>` tags.

| Option (`prop`) | Description                         | Required? | Example Value(s)          |
| :-------------- | :---------------------------------- | :-------- | :------------------------ |
| `href`          | The web address (URL) the button links to. | Yes       | `/about`, `/pricing/pro`, `https://google.com` |
| `variant`       | The style of the button.            | No        | `primary`, `secondary`, `outline`, `ghost`, `link`, `destructive` (Default: `primary`) |
| `size`          | The size of the button.             | No        | `default`, `sm`, `lg`, `icon` (Default: `default`) |
| `children`      | The text displayed *inside* the button. | Yes       | Put text between tags |

## Example MDX Usage

**Simple Primary Button:**
```mdx
<Button href="/features">See Features</Button>
```

**Secondary Button Linking Externally:**
```mdx
<Button href="https://example.com" variant="secondary">Visit Example.com</Button>
```

**Outlined Button (smaller size):**
```mdx
<Button href="/pricing" variant="outline" size="sm">View Pricing</Button>
```

**Large Call-to-Action Button:**
```mdx
<Button href="/signup" size="lg">Get Started Today</Button>
```

**Ghost Button (subtle style):**
```mdx
<Button href="/docs" variant="ghost">Read Documentation</Button>
```

**Link-styled Button (looks like a link, acts like a button):**
```mdx
<Button href="/terms" variant="link">Terms & Conditions</Button>
```

**Button inside paragraph text:**
```mdx
Read our latest blog post or <Button href="/contact">Contact Us</Button> today!
```

## Button Variants Explained

- **`primary`**: Bold, primary action button with filled background (default)
- **`secondary`**: Softer style for secondary actions
- **`outline`**: Button with border, transparent background
- **`ghost`**: Minimal style, shows background only on hover
- **`link`**: Styled like a text link but with button behavior
- **`destructive`**: Red style for dangerous actions (use sparingly)

## Button Sizes

- **`default`**: Standard button size (good for most uses)
- **`sm`**: Smaller, compact button
- **`lg`**: Larger, more prominent button
- **`icon`**: Square button for icon-only content
