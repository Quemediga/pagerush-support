# PageRush Help Center: Complete Guide to Building and Managing Your Website

This article explains the main PageRush workflows: setting up your public website, creating posts and landing pages, managing images, configuring your site, connecting custom domains, handling billing, and using AI tools with PageRush.

PageRush is a website builder for publishing posts, landing pages, images, and site settings. You manage your site from the admin panel, and PageRush turns your content into a public website.

## Support Guidelines

When asking for help, include the page, post, image, domain, or billing action you are trying to complete.

For content questions, PageRush support will usually refer to Markdown or MDX. PageRush content is written as formatted text with optional metadata at the top.

For image and media questions, PageRush support will usually explain that media is uploaded to PageRush and then used by URL in Markdown or MDX.

For website visibility problems, the first thing to check is your nickname. A public PageRush website requires a permanent nickname.

For payment, plans, invoices, cancellation, and card questions, use Billing & Plans. PageRush uses Stripe as the secure payment processor.

Human support is recommended for failed payments, missing subscriptions, duplicate charges, domain verification issues after DNS setup, and account access problems.

## Account and Website Identity

### Website URL and Nickname

Your PageRush website becomes publicly accessible after you set a permanent nickname. The nickname creates your PageRush website URL, such as:

```text
https://your-nickname.pagerush.online
```

If no nickname is set, public website URLs are not available yet.

Your nickname is permanent once it is set. Choose carefully because it becomes part of your public PageRush website URL.

Premium users may also connect a custom domain.

### Password Reset

If you forgot your password, go to Profile and use the password reset option. PageRush sends a password reset link to your account email.

## Posts, Pages, and Markdown

### Create a New Page or Post

Go to Posts, choose Create New Post, and paste complete MDX content with frontmatter at the top. You can save the content as a draft or publish it.

Markdown is formatted text, similar to the formatting used in many AI chats. MDX is Markdown with optional components. PageRush uses it to create posts and landing pages from text.

### Frontmatter

Frontmatter is metadata at the top of a post between `---` lines. It can include fields like:

```yaml
---
title: "Example Page Title"
excerpt: "Short description for search engines and previews."
slug: "example-page"
date: "2026-05-13"
author: "Your Name"
tags: ["example", "page"]
image: "https://example.com/image.jpg"
imageAlt: "Description of the image"
mode: "landing-page"
---
```

Title and excerpt are strongly recommended.

Use `mode: "landing-page"` for a clean landing page layout. Use `mode: "blog-post"` for a blog-style post.

Use lowercase, hyphen-separated slugs, such as `my-service-page`.

### Headings

If the frontmatter already has a title, PageRush uses that title as the main page heading. Start the body with normal text or `##` headings to avoid duplicate H1 headings.

### Blog Posts and Landing Pages

Blog posts use a content-focused layout with metadata such as date, author, and tags.

Landing pages use a cleaner layout for offers, services, products, or campaigns.

### Drafts and Publishing

You can save a post without publishing it. Save it as a draft or use Save for Later.

Drafts stay in the admin panel and do not have a public post URL until published. If you need a public URL, publish the post first.

### Editing Posts

Open Posts, choose Edit, update the full MDX content, and save.

Keep the frontmatter format valid. Avoid changing slugs unless you intend to change the public URL.

### Deleting and Unpublishing Posts

Open Posts and use Delete to remove a post from your admin list and public site.

If you only want to hide a post, unpublish it instead.

### Featured Post

The featured post is the published post shown prominently on your homepage.

Only published posts can be featured.

## Images and Media

### Uploading Images

Upload images to the Image Library, copy the image URL, and use that URL in Markdown or MDX.

The admin image library accepts image files up to 20 MB. The upload starts automatically after you pick a file.

### Why PageRush Uses Image URLs

PageRush content is text-based. Images and media are referenced by URL inside Markdown or MDX, which keeps pages portable and easy to edit.

### Public Media URLs

Uploaded media is stored for website use and may be accessible to anyone with the file URL, even if it is not currently embedded in a published page.

Do not upload private or sensitive files unless you intend to use them with PageRush.

### Image Accessibility Text

PageRush automatically generates accessibility-friendly descriptions for uploaded images.

In storage, this description is saved as `altText`. In website content, it may be used as `imageAlt`.

This helps screen readers and improves accessibility.

### Show Image Descriptions

The Show Image Descriptions setting controls whether descriptions appear visually under images.

It does not remove accessibility text used by screen readers.

### Delete an Uploaded Image

Open Image Library and choose Delete.

If the image URL is already used in a post, remove or replace that URL in the post content too.

## Site Configuration

### Site Name and SEO Description

Go to Site Configuration, then Site Identity & SEO.

These fields control how your site appears in search engines and link previews.

### Footer

Go to Site Configuration, then Footer & Copyright.

You can customize the footer line and optional business details.

### Site Color

Go to Site Configuration, then Primary Color.

Choose a color or enter a hex value like:

```text
#7c3aed
```

PageRush generates related theme shades automatically.

### Default Language

Go to Site Configuration, then Default Language.

This affects date formatting and the HTML language attribute.

### Default Post Mode

Default Post Mode controls whether new content starts as `blog-post` or `landing-page`.

Individual posts can still override this in frontmatter.

### Advanced Configuration

You can edit raw site settings JSON in Advanced Configuration.

Only use valid JSON with double quotes. If you are unsure, ask support before saving.

## Premium Features

PageRush has two paid plans.

Essential includes unlimited posts and pages. Use Essential when you want all published content to be live and do not need advanced business features.

Premium includes unlimited posts and pages plus custom domains, marketing pixels, and the WhatsApp CTA with Carlos Alegre signature design.

Check Billing for the current plan comparison.

### Marketing Pixels

Marketing pixels are tracking snippets such as Google Analytics or Facebook Pixel.

They help you measure visits, conversions, and audience behavior.

Marketing pixels are a Premium feature.

### WhatsApp CTA Button

The WhatsApp CTA button is a Premium feature that uses a signature design by Carlos Alegre, the PageRush creator. It appears after the visitor scrolls, sits at the bottom center of the screen, stays visually prominent, and becomes wide/thumb-friendly on mobile.

It appears after scrolling and stops at the end of post content.

Use a valid WhatsApp URL such as:

```text
https://wa.me/...
https://api.whatsapp.com/...
```

PageRush normalizes supported WhatsApp URL formats automatically.

If you cannot enable WhatsApp CTA or marketing pixels, confirm that your account is on Premium.

## Custom Domains

Custom domains are available on the Premium plan.

You can use a domain like `example.com` or a subdomain like `www.example.com`.

### Connect a Custom Domain

1. Go to Custom Domain.
2. Enter your domain without `https://`.
3. Add the DNS records shown by PageRush in your domain provider.
4. Return to PageRush and click Check Verification Status.

### Main Domain or www

Try your main domain first, such as `example.com`.

If your DNS provider does not allow the required setup, use a subdomain such as `www.example.com`.

If your domain provider will not allow a CNAME pointing your main domain, you can point your `nameservers` to Cloudflare to manage your DNS records in Cloudflare, which supports it.

### Cloudflare DNS

If you are using Cloudflare to manage your DNS records, all records must be DNS-only, shown as the gray cloud, instead of proxied, shown as the orange cloud.

Do not use `www` redirect rules between your main domain and `www`.

PageRush already proxies your domain through Cloudflare.

### Required DNS Records

PageRush shows the exact DNS records in the Custom Domain page.

You may need ownership verification, SSL validation or delegation, and a CNAME pointing your domain to PageRush.

### Domain Verification Time

DNS propagation can take 24 to 48 hours.

After updating DNS, return to PageRush and click Check Verification Status.

If your custom domain still says pending, confirm that the DNS records match exactly, wait for DNS propagation, then click Check Verification Status again.

If verification still fails after 48 hours, contact support with your domain name and a screenshot of your DNS records.

### Remove a Custom Domain

Go to Custom Domain and choose Remove Domain.

You can add it again later if needed.

## Billing and Stripe

### Manage Billing

Go to Billing & Plans.

If you already have a Stripe customer account, use Manage Billing to open the Stripe billing portal.

PageRush uses Stripe for secure payments. Stripe supports major credit cards, debit cards, and various local payment methods depending on your region.

PageRush does not store full card numbers.

### Upgrade or Downgrade

You can upgrade or downgrade your plan from Billing & Plans.

Upgrades take effect immediately.

Downgrades take effect at the end of the current billing period, so you keep the plan benefits until then.

### Cancel a Subscription

Open Billing & Plans and use Manage Billing.

Cancellation takes effect through Stripe.

Your site remains active until the end of the current billing period.

### Content After Cancellation

Your posts, images, and settings remain stored in your admin panel.

After cancellation, public site access may be deactivated, but you can reactivate later to make the site public again.

### Refund Policy

PageRush offers a 7-day money-back guarantee for paid plans.

Contact support within 7 days of purchase if you need a refund.

### Invoices and Card Updates

Open Billing & Plans and choose Manage Billing.

Stripe handles invoices, payment methods, and billing details.

### Charged but Plan Did Not Update

Contact support and include:

- Account email
- Approximate charge time
- Plan selected
- Any Stripe receipt or invoice email

This should be escalated to a human.

### Failed Checkout or Payment Error

Try again with a valid payment method, or use Manage Billing if your Stripe customer account already exists.

If the problem continues, contact support with the error message and account email.

## AI and ChatGPT Integration

### Use AI to Create PageRush Content

PageRush works well with AI-generated Markdown or MDX.

Ask the AI for complete MDX with frontmatter, then paste it into the post editor.

Ask for valid MDX only: YAML frontmatter first, then Markdown content.

Tell the AI to use:

- Simple single-line frontmatter values
- Lowercase hyphenated slugs
- Either `landing-page` or `blog-post` mode

### AI-Generated Post Save Errors

Common causes of save errors include:

- Invalid frontmatter
- Multiline YAML values
- Unsupported MDX components
- Raw HTML
- Mixed image and text in the same paragraph
- Invalid Markdown

Fix the MDX and try again.

### ChatGPT App

If you enable the PageRush ChatGPT App, ChatGPT can help create posts, edit content, upload images by URL, manage drafts, and update settings.

It uses your connected PageRush account.

### ChatGPT Account Connection and Privacy

The ChatGPT integration uses basic sign-in scopes to connect the right PageRush account.

PageRush uses verified email to sync your ChatGPT session with your PageRush account.

MCP tools do not return your email, payment identifiers, passwords, or tokens.

## Troubleshooting

### Cannot Log In

Try resetting your password from Profile or the login screen.

If you still cannot access the account, contact support with your account email.

### Site URL Does Not Work

Confirm that:

- Your nickname is set
- The post is published
- The post has a category and slug

Drafts do not have public URLs.

### Published Post Is Not Showing

Confirm the post status is Published in Posts.

If you recently changed the slug, use the new URL.

If you are using a custom domain, verify the domain is active.

If you are using PageRush through this AI integration without a paid plan, your account includes 1 free-of-cost live post. That post defaults to the newest created or edited published post. Essential unlocks unlimited live posts and pages. Premium also adds custom domains, marketing pixels, and the WhatsApp CTA with Carlos Alegre signature design.

### Broken Image

Confirm the image URL opens in a browser.

If you deleted the image from the Image Library, replace or remove the old URL in the post content.

### Custom Domain Is Active but Site Still Does Not Load

Check DNS propagation, SSL status, and whether the exact domain or subdomain is connected.

If it remains broken after 48 hours, escalate to support.

## When to Contact Human Support

Contact PageRush Support when the issue involves:

- Billing disputes
- Refunds after unclear payment status
- Duplicate charges
- Missing paid plan access
- Domain verification failures after 48 hours
- Account access issues
- Suspected security issues
- Any request involving private account investigation
