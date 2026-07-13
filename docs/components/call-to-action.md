# Component: CallToAction (CTA)

## Purpose
Creates a distinct block designed to grab attention and encourage the user to take a specific action (like signing up, learning more, etc.). Usually contains text and one or two buttons.

## When to Use
* At the end of a page or section to prompt the next step.
* Highlighting a key offer or benefit.
* Driving sign-ups, downloads, or contact requests.

## How to Use (Options / Props)

| Option (`prop`) | Description                                     | Required?      | Example Value(s)                  |
| :-------------- | :---------------------------------------------- | :------------- | :-------------------------------- |
| `title`         | The main headline for the CTA block.            | Yes            | `"Ready to Start?"`, `"Get Your Free Trial"` |
| `description`   | Short text explaining the offer or action.      | Yes            | `"Sign up today and get..."`     |
| `button1Text`   | Text for the primary action button.             | Yes            | `"Sign Up Now"`, `"Learn More"`   |
| `button1Href`   | URL link for the primary action button.         | Yes            | `/signup`, `/features`            |
| `button2Text`   | Text for an optional secondary action button.   | No             | `"Book a Demo"`, `"Read Docs"`    |
| `button2Href`   | URL link for the optional secondary button.     | No (Yes if `button2Text` is used) | `/demo`, `/docs`                  |
| `children`      | Optional extra text below buttons.              | No             | Put text between tags            |

## Example MDX Usage

**CTA with one button:**
```mdx
<CallToAction
  title="Get Started Today!"
  description="Join thousands of users benefiting from our service. No credit card required for trial."
  button1Text="Start Free Trial"
  button1Href="/signup"
/>
```

**CTA with two buttons and extra text:**
```mdx
<CallToAction
  title="Explore Our Powerful Features"
  description="See how our tools can help you achieve your goals faster."
  button1Text="View Features"
  button1Href="/features"
  button2Text="Request a Demo"
  button2Href="/request-demo"
>
  *14-day free trial available on all plans.*
</CallToAction>
```
