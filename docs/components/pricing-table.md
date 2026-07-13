# Component: PricingTable

## Purpose
Displays different pricing plans or tiers side-by-side, usually in columns, making it easy for users to compare options.

## When to Use
* On a pricing page.
* On a landing page to show available subscription options.

## How to Use (Options / Props)

This component takes a single `plans` prop, which needs to be a list (an "array") of plan details.

| Option (`prop`) | Description                                                                                                | Required? | Example Value Format                                                                                                                                                                                                                                                                                                                         |
| :-------------- | :--------------------------------------------------------------------------------------------------------- | :-------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `plans`         | A list where each item describes a pricing plan. Each plan *object* within the list needs the keys below. | Yes       | `{[ { plan details 1 }, { plan details 2 } ]}`                                                                                                                                                                                                                                                                                                            |

**Each Plan Object within the `plans` list needs these keys:**

| Key in Plan Object | Description                                        | Required?       | Example Value(s)                     |
| :----------------- | :------------------------------------------------- | :-------------- | :----------------------------------- |
| `name`             | Name of the pricing tier (e.g., "Basic", "Pro").   | Yes             | `"Free"`, `"Professional"`           |
| `price`            | The price amount.                                  | Yes             | `"$0"`, `"$49.99"`                   |
| `frequency`        | How often the price is charged (e.g., per month).  | Yes             | `"/month"`, `"/year"`, `"one-time"`   |
| `features`         | A list of features included in this plan.          | Yes             | `['Feature A', 'Feature B', '10 Users']` |
| `buttonText`       | Text for the action button for this plan.          | Yes             | `"Sign Up"`, `"Get Started"`         |
| `buttonHref`       | URL link for the action button.                    | Yes             | `/signup/free`, `/checkout/pro`      |
| `isFeatured`       | Set to `true` to visually highlight this plan.     | No (Default: `false`) | `true`, `false`                  |

**Important:** This component requires structured data. Ensure the AI formats the `plans` prop correctly as a list of objects, with each object containing all the required keys.

## Example MDX Usage

```mdx
<PricingTable plans={[
  {
    name: 'Starter',
    price: '$0',
    frequency: '/month',
    features: [
      '1 Project',
      'Basic Analytics',
      'Community Support'
    ],
    buttonText: 'Get Started',
    buttonHref: '/signup/starter'
  },
  {
    name: 'Business',
    price: '$29',
    frequency: '/month',
    features: [
      'Unlimited Projects',
      'Advanced Analytics',
      'Email Support',
      'Team Collaboration'
    ],
    buttonText: 'Choose Business',
    buttonHref: '/signup/business',
    isFeatured: true
  },
  {
    name: 'Enterprise',
    price: 'Custom',
    frequency: '',
    features: [
      'All Business Features',
      'Dedicated Account Manager',
      'Premium Support',
      'Custom Integrations'
    ],
    buttonText: 'Contact Sales',
    buttonHref: '/contact/sales'
  }
]} />
```
