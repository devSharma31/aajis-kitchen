# Aaji's Kitchen — restaurant landing page (concept)

A mobile-first landing page for a fictional family-run Maharashtrian restaurant in Sadashiv Peth, Pune. It's built around one action: **order direct on WhatsApp and save 10%** instead of going through a delivery app.

**Live:** [aajis-kitchen.vercel.app](https://aajis-kitchen.vercel.app) · [GitHub Pages](https://devsharma31.github.io/aajis-kitchen/)

> Concept project for my design portfolio. The business, prices, ratings, address and phone number are fictional, and the reviews are labelled as samples.

---

## The brief

| | |
|---|---|
| **Business** | Family-run Maharashtrian restaurant, budget to mid-range |
| **Customers** | Families, office groups and repeat local customers |
| **Goal** | Order direct on WhatsApp, with a "10% off when you order direct" offer |
| **Brand feel** | Homely, warm, traditional |

## The real problems, and how the page solves them

| Problem | Fix on the page |
|---|---|
| **Delivery apps take 25–30% commission** on every order | The whole page pushes ordering direct. The 10% offer is in the first thing you read, and the main button leads to the menu. |
| **Regulars don't know they can order direct**, or that it's cheaper | A side-by-side example: the same family order for 4 costs ₹1,180 on an app and ₹936 direct. |
| **Weekend table waits push people away** | A "Skip the queue" box: send "TABLE for 4" on WhatsApp and get a message when your table is nearly ready. |

## The key feature: a menu that writes your order

Every dish has a photo, a price in ₹ and an **Add** button. As you add dishes, a running total shows the subtotal, the 10% saving and the final amount. One tap sends a WhatsApp message listing every item, quantity and total. The restaurant gets a complete order with no back-and-forth.

## Design decisions

- **Section order:** offer (hero) → *why direct?* (price comparison) → menu → *is it easy?* (3 steps) → family story and hygiene (FSSAI registration, fresh oil daily, Jain/fasting options) → weekend queue → reviews → hours and map → FAQ → final CTA.
- **Colour:** rice-paper cream `#FFF8EC` with dark brown `#2A1C13` text (15.6:1). **Kokum red `#9E1F28` is used only on buttons** (7.8:1). Leaf green marks vegetarian items and savings.
- **Type:** Rozha One for headings, with Devanagari-inspired forms for a traditional feel, and Mukta for body text, which also supports Marathi.

## Conversion review (second pass)

I reviewed the first version from two sides: a busy customer on a phone with a slow connection, and the owner who wants more direct orders.

| Issue found | Change |
|---|---|
| **The "Find us on" cards linked to Zomato and Swiggy**, sending customers to the apps that take the commission | Turned into non-clickable rating badges, with a note: "The same food is on Zomato and Swiggy, priced higher to cover their commission. Ordering here costs 10% less." |
| Hero button said "Order on WhatsApp" but scrolled to the menu | Relabelled "See menu & order — 10% off", so it does what it says |
| Five-line intro paragraph | Cut to two lines; the main button moved up from 532px to 473px on a 375×667 screen |
| Google Fonts blocked the first paint on slow connections | Fonts load in the background |
| Generic copy ("Hungry?", "Easier than an app. Really.") | Replaced with specific lines ("No app, no login, three steps") |

## Accessibility and performance

- Semantic HTML, labelled +/– buttons that announce each dish, live-updating order total for screen readers
- All text passes WCAG AA contrast
- 12 dish thumbnails at 160px, all lazy-loaded, with styled fallbacks if an image fails
- No frameworks: one HTML file with inline CSS and vanilla JavaScript
- SEO: meta description, Open Graph tags, and `Restaurant` JSON-LD structured data

## What I'd test next with real customers

1. **How to show the offer:** "10% off" vs "Save ₹100+ on a family order". Which gets more dishes added?
2. **Cart completion.** How many people add dishes but never send the order?
3. **A Marathi headline** for long-time Sadashiv Peth regulars.

## Stack

HTML · CSS · vanilla JavaScript · Google Fonts · Unsplash photos · Simple Icons (CC0) · deployed on GitHub Pages and Vercel

## How this was built

I built this with Claude (Anthropic's AI assistant) as a design and coding partner.

**My part:** I wrote the business brief and page requirements, reviewed every version, asked for revisions (verified photos, a photo for every dish, real brand logos), commissioned the conversion review above, and published the site to GitHub and Vercel.

**Claude's part:** it wrote the HTML, CSS, JavaScript and copy to that brief.

---

Concept design by Devashish Sharma. Fictional business.
