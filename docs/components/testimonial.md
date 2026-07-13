# Component: Testimonial

## Purpose
Displays a quote from a customer, user, or expert to build trust and social proof.

## When to Use
* On landing pages to show customer satisfaction.
* On product pages to highlight positive feedback.
* Anywhere you want to showcase endorsements.

## How to Use (Options / Props)

| Option (`prop`) | Description                         | Required? | Example Value(s)                  |
| :-------------- | :---------------------------------- | :-------- | :-------------------------------- |
| `quote`         | The actual text of the testimonial. | Yes       | `"This product changed my life!"` |
| `authorName`    | The name of the person quoted.      | Yes       | `"Jane Doe"`                      |
| `authorTitle`   | The title or company of the person. | No        | `"CEO, Example Inc."`, `"Happy Customer"` |
| `avatarSrc`     | URL path to an image of the author. | No        | `/images/avatars/jane.jpg`        |
| `children`      | Optional extra text/notes inside.   | No        | Put text between tags            |

## Example MDX Usage

**Basic Testimonial:**
```mdx
<Testimonial
  quote="Using this service was the best decision we made this year. Highly recommended!"
  authorName="John Smith"
  authorTitle="Marketing Manager, Globex Corp"
/>
```

**Testimonial with Avatar and extra note:**
```mdx
<Testimonial
  quote="Incredible results in just the first month. The support team is fantastic too."
  authorName="Alice Green"
  authorTitle="Founder, Startup Hub"
  avatarSrc="/images/avatars/alice.png"
>
  *Results may vary.*
</Testimonial>
```
