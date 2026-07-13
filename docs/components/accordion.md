# Component: Accordion

## Purpose
Creates a list of collapsible sections, often used for Frequently Asked Questions (FAQs) or organizing detailed information concisely. Users click a title to reveal the content.

## When to Use
* Displaying FAQs.
* Hiding detailed steps or explanations until needed.
* Organizing complex information into manageable chunks.

## How to Use (Options / Props)

This component takes a single `items` prop, which needs to be a list (an "array") of questions and answers.

| Option (`prop`) | Description                                                                                                | Required? | Example Value Format                                                                                                                               |
| :-------------- | :--------------------------------------------------------------------------------------------------------- | :-------- | :------------------------------------------------------------------------------------------------------------------------------------------------- |
| `items`         | A list where each item has a `title` (the clickable part) and `content` (the hidden part that gets revealed). | Yes       | `{[ { title: 'Question 1', content: 'Answer 1' }, { title: 'Question 2', content: 'Answer 2 can include **Markdown**.' } ]}` |

**Important:** The `content` for each item can contain Markdown formatting (like bold, italics, links, lists). Make sure the AI you use knows how to format the `items` prop correctly as shown in the example.

## Example MDX Usage

```mdx
<Accordion items={[
  {
    title: 'What is MDX?',
    content: 'MDX is Markdown that allows you to use JSX components like this Accordion directly within your content.'
  },
  {
    title: 'How do I add another question?',
    content: 'Just add another object `{ title: "New Question", content: "New Answer" }` to the `items` list, separated by a comma.'
  },
  {
    title: 'Can the content have formatting?',
    content: 'Yes! The `content` can include:\n\n* Lists\n* **Bold text**\n* [Links](https://example.com)\n* And more Markdown features.'
  }
]} />
```
