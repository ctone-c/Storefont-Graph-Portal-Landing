# Storefront Graph Portal — Landing Page

A developer portal landing page for **Storefront Graph** (formerly Federated Graph), Volvo Cars' unified GraphQL API for building customer and retailer experiences.

Built with the [`@volvo-cars/css`](https://www.npmjs.com/package/@volvo-cars/css) v1.51.0 design system — no framework, plain HTML + CSS.

---

## Overview

The page gives developers a single entry point to discover, explore, and integrate with the Storefront Graph API. It includes:

| Section | Description |
|---|---|
| **Hero** | Portal identity — logo, title, and primary CTAs to open the Explorer or jump to Quick Start |
| **Quick Links** | Four cards linking to Explore queries, Read the docs, Register your client, and Try live examples |
| **Quick Start** | Three-step guide — build a query, register a client, send a request (with JS / cURL / Java code tabs) |
| **Need Help** | Escalation guide for raising issues with the correct domain or platform team |
| **Data & Domains** | Overview of the six data domains available in the graph |
| **Footer** | Contact, resources, and contributor links |

---

## Features

- **Light / Dark theme toggle** — persisted to `localStorage`, no flash on page load
- **Fully responsive** — 1 → 2 → 4 column layouts at design system breakpoints (520 px, 1024 px)
- **Accessible** — ARIA landmark labels, semantic HTML, sufficient colour contrast in both themes
- **Design system tokens** — spacing, colours, typography, and radius all use `--v-*` CSS custom properties

---

## Getting Started

No build step required. Open `index.html` directly in a browser, or serve the folder with any static server:

```bash
npx serve .
# or
python3 -m http.server 8080
```

Then visit `http://localhost:8080` (or whichever port is shown).

---

## Prerequisites

The page loads the Volvo Cars design system CSS from the local `node_modules` folder. Install dependencies before opening:

```bash
npm install
# or
yarn
```

---

## Project Structure

```
index.html                          # Full portal page (single file)
storefront-graph-apple-touch-icon.png  # Portal logo (used in hero)
storefront_placeholder.png          # Placeholder image for quick-link cards
package.json                        # Lists @volvo-cars/css dependency
```

---

## Design System

This page uses [`@volvo-cars/css`](https://www.npmjs.com/package/@volvo-cars/css) utility classes and CSS custom properties:

- **Components**: `.title-page`, `.title-section`, `.text-card`, `.callout`, `.button-filled`, `.button-outlined`, `.button-text`, `.button-group`, `.wordmark`, `.list`
- **Layout**: `.container`, `.container-md`, `.container-sm`
- **Dark mode**: `data-color-mode="light" | "dark"` on the `<html>` element

---

## Contributing

This is an internal Volvo Cars developer portal page. For changes to the Storefront Graph API, schema, or platform, reach out via the Slack `#storefront-graph` channel or submit an issue through the Explorer.
