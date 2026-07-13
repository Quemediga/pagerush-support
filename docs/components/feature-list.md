# Component: FeatureList

## Purpose
Presents a list of key features, benefits, or items in a visually appealing way, often more structured than a simple bulleted list. (This version uses text-based descriptions).

## When to Use
* Highlighting product or service features on a landing page.
* Summarizing key benefits.
* Listing steps in a process (if simple).

## How to Use (Options / Props)

This component takes a single `items` prop, which needs to be a list (an "array") of features.

| Option (`prop`) | Description                                                                               | Required? | Example Value Format                                                                              |
| :-------------- | :---------------------------------------------------------------------------------------- | :-------- | :---------------------------------------------------------------------------------------------- |
| `items`         | A list where each item has a `title` (the feature name) and `description` (a short explanation). | Yes       | `{[ { title: 'Feature 1', description: 'Desc 1' }, { title: 'Feature 2', description: 'Desc 2' } ]}` |

## Example MDX Usage

```mdx
<FeatureList items={[
  {
    title: 'Easy Integration',
    description: 'Connect with your existing tools in minutes with our straightforward setup process.'
  },
  {
    title: 'Real-time Analytics',
    description: 'Track your progress and gain valuable insights with our up-to-the-second data reporting.'
  },
  {
    title: '24/7 Support',
    description: 'Our dedicated support team is always available to help you whenever you need assistance.'
  }
]} />
```
