# Saffron & Stone — restaurant website demo

A polished, responsive React + TypeScript website for demonstrating a premium restaurant experience. The brand, menu, opening times, photographs and prices are all sample content. Replace them with verified client information before launch.

## Run locally

1. Install Node.js 20 or newer.
2. Run `npm install`.
3. Run `npm run dev` and open the local Vite URL.
4. Run `npm run build` for a production build; `npm run preview` serves that build locally.

The project uses Vite, React, TypeScript, Tailwind CSS 4, Framer Motion and Lucide icons. No database, payment provider, backend or environment variables are currently required. No server secrets belong in frontend code.

## Customization

- Edit the `dishes` and `categories` arrays, sample restaurant copy, gallery images and presentation in `src/site.tsx`.
- Change colors, typography, layout and responsive styles in `src/style.css`.
- Update page title, description, social metadata, image and structured data in `index.html`.
- Replace Unsplash image URLs with restaurant-owned or appropriately licensed images. Add descriptive alt text.
- Search for `SAMPLE`, `sample`, and `to be added` in the source before deploying. Supply verified business name, address, phone, WhatsApp, opening hours, dietary and allergen details, policies and social links.

## Interactive demo behavior and production connections

- Menu categories, search, item quantity controls, subtotal, cart drawer and gallery lightbox work in the browser. Cart state is demo-only and clears on reload.
- The reservation and event forms validate required fields and non-past dates, but only display a local demo success state. Connect a server endpoint, persist records and return a real acknowledgement before describing a request as received or confirmed.
- The cart opens a WhatsApp Web message with the item details and subtotal. It intentionally uses the generic `wa.me` share entry point because a restaurant number has not been supplied. Set a verified destination number, show delivery/pickup, delivery address, configurable charges and operating rules, and have staff/backend confirm availability. No payment is collected.
- Add a protected server-side admin, authenticated staff roles, database schema, input validation, rate limits, email/message delivery, booking-capacity conflict checks, order state, privacy/retention policies, and monitoring before using this as a live operations system. Keep credentials in server environment variables.
- Add verified review content only with the restaurant's approval. Add terms and a real privacy policy before collecting customer information in production.

## Deployment

Deploy the static `dist/` output to any Vite-compatible static host. Configure SPA fallback to `index.html` if routes are added. The current single-page site has no backend services or environment variables. Add a generated sitemap and accurate `robots.txt`, canonical URL, verified Restaurant/LocalBusiness address, hours, telephone and menu structured data when the production domain and business details are known. External fonts and Unsplash sample photos require internet access.

This site makes no search ranking or customer growth guarantees.
