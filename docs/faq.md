# PageRush Support FAQ

Use this FAQ to train or seed the PageRush support chatbot. Answers should be concise, practical, and focused on helping the user finish the task inside PageRush.

Keep this FAQ focused on the PageRush website builder, public sites, content, media, domains, billing, and account support. Do not introduce unrelated program topics.

## Account and Website Identity

### Q: What is PageRush?
A: PageRush is a website builder for publishing posts, landing pages, images, and site settings. You manage your site from the admin panel, and PageRush turns your content into a public website.
Tags: overview, getting-started

### Q: Why is my website not live yet?
A: Your PageRush website becomes publicly accessible after you set a permanent nickname. The nickname creates your PageRush website URL, such as `your-nickname.pagerush.online`. If no nickname is set, public website URLs are not available yet.
Tags: nickname, website-live, public-url

### Q: Can I change my nickname later?
A: No. Your nickname is permanent once it is set. Choose carefully because it becomes part of your public PageRush website URL.
Tags: nickname, account

### Q: What is my PageRush website URL?
A: Your default website URL is based on your nickname, usually `https://your-nickname.pagerush.online`. Premium users may also connect a custom domain.
Tags: website-url, nickname, custom-domain

### Q: I forgot my password. What should I do?
A: Go to Profile and use the password reset option. PageRush sends a password reset link to your account email.
Tags: login, password, profile

## Posts, Pages, and Markdown

### Q: How do I create a new page or post?
A: Go to Posts, choose Create New Post, and paste complete MDX content with frontmatter at the top. You can save it as a draft or publish it.
Tags: posts, create, mdx

### Q: What is MDX or Markdown?
A: Markdown is formatted text, similar to the formatting used in many AI chats. MDX is Markdown with optional components. PageRush uses it to create posts and landing pages from text.
Tags: markdown, mdx, content

### Q: What is frontmatter?
A: Frontmatter is metadata at the top of a post between `---` lines. It can include fields like title, excerpt, slug, date, author, tags, image, imageAlt, and mode.
Tags: frontmatter, mdx, seo

### Q: What frontmatter should I use?
A: Title and excerpt are strongly recommended. Use `mode: "landing-page"` for a clean landing page layout or `mode: "blog-post"` for a blog-style post. Use lowercase, hyphen-separated slugs.
Tags: frontmatter, seo, mode

### Q: Why should I avoid an H1 inside the post body?
A: If the frontmatter already has a title, PageRush uses that title as the main page heading. Start the body with normal text or `##` headings to avoid duplicate H1 headings.
Tags: headings, mdx, seo

### Q: What is the difference between a blog post and a landing page?
A: Blog posts use a content-focused layout with metadata such as date, author, and tags. Landing pages use a cleaner layout for offers, services, products, or campaigns.
Tags: posts, landing-page, blog-post

### Q: Can I save a post without publishing it?
A: Yes. Save it as a draft or use Save for Later. Drafts stay in the admin panel and do not have a public post URL until published.
Tags: drafts, publishing

### Q: Why can't I get a public URL for my draft?
A: Drafts are not public. Publish the post first, then PageRush can provide a public URL.
Tags: drafts, public-url, publishing

### Q: How do I edit an existing post?
A: Open Posts, choose Edit, update the full MDX content, and save. Keep the frontmatter format valid and avoid changing slugs unless you intend to change the public URL.
Tags: edit, posts, mdx

### Q: Can I delete a post?
A: Yes. Open Posts and use Delete. Deleting a post removes it from your admin list and public site. If you only want to hide it, unpublish it instead.
Tags: delete, posts, unpublish

### Q: What does "featured post" mean?
A: The featured post is the published post shown prominently on your homepage. Only published posts can be featured.
Tags: featured-post, homepage, publishing

## Images and Media

### Q: How do images work in PageRush?
A: Upload images to the Image Library, copy the image URL, and use that URL in Markdown/MDX. PageRush automatically generates accessibility-friendly descriptions for screen readers.
Tags: images, media, markdown

### Q: What file types can I upload?
A: The admin image library accepts image files up to 20 MB. The upload starts automatically after you pick a file.
Tags: images, upload, file-types

### Q: Why does PageRush use image URLs?
A: PageRush content is text-based. Images and media are referenced by URL inside Markdown/MDX, which keeps pages portable and easy to edit.
Tags: images, media, markdown

### Q: Are uploaded images public?
A: Uploaded media is stored for website use and may be accessible to anyone with the file URL, even if it is not currently embedded in a published page. Do not upload private or sensitive files unless you intend to use them with PageRush.
Tags: images, privacy, public-url

### Q: What is imageAlt or altText?
A: PageRush generates an accessibility description for uploaded images. In storage it is saved as `altText`; in website content it may be used as `imageAlt`. This helps screen readers and improves accessibility.
Tags: accessibility, images, alt-text

### Q: Does hiding image descriptions affect screen readers?
A: No. The "Show Image Descriptions" setting controls whether descriptions appear visually under images. It does not remove accessibility text used by screen readers.
Tags: accessibility, images, settings

### Q: Can I delete an uploaded image?
A: Yes. Open Image Library and choose Delete. If the image URL is already used in a post, remove or replace that URL in the post content too.
Tags: images, delete

## Site Configuration

### Q: Where do I change my site name and SEO description?
A: Go to Site Configuration, then Site Identity & SEO. These fields control how your site appears in search engines and link previews.
Tags: seo, settings, site-configuration

### Q: Where do I change the footer?
A: Go to Site Configuration, then Footer & Copyright. You can customize the footer line and optional business details.
Tags: footer, settings

### Q: How do I change my site color?
A: Go to Site Configuration, then Primary Color. Choose a color or enter a hex value like `#7c3aed`. PageRush generates related theme shades automatically.
Tags: color, design, settings

### Q: How do I change the default language?
A: Go to Site Configuration, then Default Language. This affects date formatting and the HTML language attribute.
Tags: language, settings

### Q: What is the default post mode?
A: Default Post Mode controls whether new content starts as `blog-post` or `landing-page`. Individual posts can still override this in frontmatter.
Tags: post-mode, settings

### Q: Can I edit raw site settings JSON?
A: Yes. Use Advanced Configuration in Site Configuration. Only use valid JSON with double quotes. If you are unsure, ask support before saving.
Tags: advanced-settings, json

## Premium Features

### Q: What is included in the Essential plan?
A: Essential includes unlimited posts and pages. It is the right paid plan when the user wants all published content to be live but does not need custom domains, marketing pixels, or the WhatsApp CTA floating button.
Tags: essential, plans, billing

### Q: What features are included in Premium?
A: Premium includes unlimited posts and pages plus professional features such as custom domains, marketing pixels, and the WhatsApp CTA with Carlos Alegre signature design. Check Billing for the current plan comparison.
Tags: premium, plans

### Q: What are marketing pixels?
A: Marketing pixels are tracking snippets such as Google Analytics or Facebook Pixel. They help you measure visits, conversions, and audience behavior. This is a Premium feature.
Tags: marketing-pixels, premium, analytics

### Q: What is the WhatsApp CTA button?
A: The WhatsApp CTA button is a Premium feature using a signature design by Carlos Alegre, the PageRush creator. It appears only on post pages after the visitor scrolls, sits at the bottom center of the screen, stays visually prominent, and is wide/thumb-friendly on mobile so it falls naturally below the visitor's thumb.
Tags: whatsapp, premium, cta

### Q: What WhatsApp URL format should I use?
A: Use a valid `https://wa.me/...` or `https://api.whatsapp.com/...` URL. PageRush normalizes supported WhatsApp URL formats automatically.
Tags: whatsapp, settings

### Q: Why can't I enable WhatsApp CTA or marketing pixels?
A: These are Premium features. Upgrade to Premium from Billing to enable them.
Tags: premium, whatsapp, marketing-pixels

## Custom Domains

### Q: Can I use my own domain?
A: Yes, custom domains are available on the Premium plan. You can use a domain like `example.com` or a subdomain like `www.example.com`.
Tags: custom-domain, premium

### Q: How do I connect a custom domain?
A: Go to Custom Domain, enter your domain without `https://`, add the DNS records shown by PageRush in your domain provider, then return to PageRush and click Check Verification Status.
Tags: custom-domain, dns

### Q: Should I connect my main domain or www?
A: Try your main domain first, such as `example.com`. If your DNS provider does not allow the required setup, use a subdomain such as `www.example.com`.
Tags: custom-domain, dns

### Q: What DNS records do I need?
A: PageRush shows the exact DNS records in the Custom Domain page. You may need ownership verification, SSL validation or delegation, and a CNAME pointing your domain to PageRush.
Tags: custom-domain, dns, ssl

### Q: How long does domain verification take?
A: DNS propagation can take 24 to 48 hours. After updating DNS, return to PageRush and click Check Verification Status.
Tags: custom-domain, dns, verification

### Q: My custom domain still says pending. What should I do?
A: Confirm that the DNS records match exactly, wait for DNS propagation, then click Check Verification Status. If it still fails after 48 hours, contact support with your domain name and a screenshot of your DNS records.
Tags: custom-domain, troubleshooting, escalation

### Q: Can I remove a custom domain?
A: Yes. Go to Custom Domain and choose Remove Domain. You can add it again later if needed.
Tags: custom-domain, remove

### Q: My main domain won't connect, what can I do?
A: If your domain provider won't allow a CNAME pointing your main domain, you can point your `nameservers` to Cloudflare to manage your DNS records in Cloudflare, which supports it.
Tags: custom-domain, dns

### Q: My domain from Cloudflare doesn't work?
A: If you are using Cloudflare to manage you DNS records, all records must be "DNS-only" (gray cloud) instead of "proxied" (orange cloud). You should not use `www` or redirect rules between your main domain and `www`. PageRush already proxies your domain through Cloudflare.
Tags: custom-domain, dns

## Billing and Stripe

### Q: Where do I manage billing?
A: Go to Billing & Plans. If you already have a Stripe customer account, use Manage Billing to open the Stripe billing portal.
Tags: billing, stripe

### Q: What payment methods are accepted?
A: PageRush uses Stripe for secure payments. Stripe supports major credit cards, debit cards, and various local payment methods depending on your region. PageRush does not store full card numbers.
Tags: billing, payment-methods, stripe

### Q: Can I upgrade or downgrade my plan?
A: Yes. Upgrades take effect immediately. Downgrades take effect at the end of the current billing period, so you keep the plan benefits until then.
Tags: billing, plans, upgrade, downgrade

### Q: Can I cancel my subscription?
A: Yes. Open Billing & Plans and use Manage Billing. Cancellation takes effect through Stripe. Your site remains active until the end of the current billing period.
Tags: billing, cancellation, stripe

### Q: What happens to my content if I cancel?
A: Your posts, images, and settings remain stored in your admin panel. After cancellation, public site access may be deactivated, but you can reactivate later to make the site public again.
Tags: billing, cancellation, content

### Q: Is there a refund policy?
A: PageRush offers a 7-day money-back guarantee for paid plans. Contact support within 7 days of purchase if you need a refund.
Tags: billing, refund

### Q: Where can I find invoices or update my card?
A: Open Billing & Plans and choose Manage Billing. Stripe handles invoices, payment methods, and billing details.
Tags: billing, invoice, stripe

### Q: I was charged but my plan did not update. What should I do?
A: Contact support and include the account email, approximate charge time, plan selected, and any Stripe receipt or invoice email. This should be escalated to a human.
Tags: billing, stripe, escalation

### Q: I see a failed checkout or payment error. What should I do?
A: Try again with a valid payment method, or use Manage Billing if your Stripe customer account already exists. If the problem continues, contact support with the error message and account email.
Tags: billing, checkout, stripe, troubleshooting

## AI and ChatGPT Integration

### Q: Can I use AI to create PageRush content?
A: Yes. PageRush works well with AI-generated Markdown/MDX. Ask the AI for complete MDX with frontmatter, then paste it into the post editor.
Tags: ai, mdx, content

### Q: What should I ask AI to generate?
A: Ask for valid MDX only: YAML frontmatter first, then Markdown content. Tell it to use simple single-line frontmatter values, lowercase hyphenated slugs, and either `landing-page` or `blog-post` mode.
Tags: ai, prompt, mdx

### Q: Why did my AI-generated post fail to save?
A: Common causes are invalid frontmatter, multiline YAML values, unsupported MDX components, raw HTML, mixed image and text in the same paragraph, or invalid Markdown. Fix the MDX and try again.
Tags: ai, mdx, troubleshooting

### Q: Can ChatGPT manage my PageRush site?
A: If you enable the PageRush ChatGPT App, ChatGPT can help create posts, edit content, upload images by URL, manage drafts, and update settings. It uses your connected PageRush account.
Tags: chatgpt, ai, mcp

### Q: Does ChatGPT need my email?
A: The ChatGPT integration uses basic sign-in scopes to connect the right PageRush account. PageRush uses verified email to sync your ChatGPT session with your PageRush account. MCP tools do not return your email, payment identifiers, passwords, or tokens.
Tags: chatgpt, privacy, account

## Troubleshooting and Escalation

### Q: I cannot log in. What should I do?
A: Try resetting your password from Profile or the login screen. If you still cannot access the account, contact support with your account email.
Tags: login, troubleshooting, escalation

### Q: My site URL does not work. What should I check?
A: Confirm that your nickname is set, the post is published, and the post has a category and slug. Drafts do not have public URLs.
Tags: public-url, nickname, publishing

### Q: My published post is not showing.
A: Confirm the post status is Published in Posts. If you recently changed the slug, use the new URL. If using a custom domain, verify the domain is active.
Tags: posts, publishing, custom-domain

### Q: Why are only some of my posts live when I use PageRush through this AI integration?
A: Users managing PageRush through this AI integration get special free access with 1 free-of-cost live post. That free live post is the newest created or edited published post. Essential unlocks unlimited live posts and pages. Premium also adds custom domains, marketing pixels, and the WhatsApp CTA with Carlos Alegre signature design.
Tags: ai, free-access, plans, publishing

### Q: My image is broken on the page.
A: Confirm the image URL opens in a browser. If you deleted the image from the Image Library, replace or remove the old URL in the post content.
Tags: images, troubleshooting

### Q: My custom domain is active but the site still does not load.
A: Check DNS propagation, SSL status, and whether the exact domain or subdomain is connected. If it remains broken after 48 hours, escalate to support.
Tags: custom-domain, dns, escalation

### Q: When should an AI assistant recommend contacting human support?
A: Escalate billing disputes, refunds after unclear payment status, duplicate charges, missing paid plan access, domain verification failures after 48 hours, account access issues, suspected security issues, and any request involving private account investigation.
Tags: escalation, support-policy
