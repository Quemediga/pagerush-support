# Component: Card

## Purpose
Displays information in a self-contained box, often with an image, title, description, and a link. Good for summaries or previews.

## When to Use
* Previewing blog posts or articles.
* Highlighting key features or services briefly.
* Showcasing team members or portfolio items.
* Grouping related links or resources.

## How to Use (Options / Props)

The main description or content goes between the opening `<Card>` and closing `</Card>` tags.

| Option (`prop`) | Description                                   | Required? | Example Value(s)              |
| :-------------- | :-------------------------------------------- | :-------- | :---------------------------- |
| `title`         | The main heading for the card.                | Yes       | `"Our Latest Blog Post"`      |
| `href`          | The URL the card links to when clicked.       | No        | `/blog/latest`, `/features/x` |
| `imageSrc`      | URL path to an optional image for the card.   | No        | `/images/cards/post.jpg`      |
| `children`      | The main description text inside the card.    | Yes       | Put text between tags        |

## Example MDX Usage

**Card with Title, Text, and Link:**
```mdx
<Card title="Explore Our Services" href="/services">
  Discover the wide range of solutions we offer to help your business grow.
</Card>
```

**Card with Image, Title, Text, and Link:**
```mdx
<Card title="New Feature Announced!" href="/blog/new-feature" imageSrc="/images/cards/feature-x.png">
  We've just launched an exciting new feature. Click here to learn all about it and how it can benefit you.
</Card>
```

**Card without a link (just info):**
```mdx
<Card title="Important Update">
  Please note that our scheduled maintenance will occur this Sunday.
</Card>
```
