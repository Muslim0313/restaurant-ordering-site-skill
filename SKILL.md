---
name: restaurant-ordering-site
description: Build, revise, and publish a restaurant ordering website when the owner supplies a menu, prices, food references, delivery rules, and brand feedback. Use for menu sites with carts and order handoff; adapt the design and workflow to each restaurant.
---

# Restaurant ordering site

Turn the restaurant owner's actual menu and visual references into a usable ordering site. Keep the owner's current instructions authoritative over earlier drafts and over generic examples.

## Menu and ordering

- Treat owner-provided names, prices, portions, delivery areas, address, and contact details as source data. Update only the items the owner changes; preserve unmentioned prices and items.
- Distinguish products with similar names across categories, such as a roll and a pizza. Give each a stable identifier, category, image, and price. For variable-price dishes, display the range and explain how the final amount is confirmed before an order is sent.
- Organize a long menu with clear category headings and filters. Make product cards easy to scan on a phone, with visible name, price, image, and add-to-cart control. Let a tap on the image open a larger view when requested.
- Keep delivery and pickup options accurate. If delivery is limited to named places, show the permitted places at the address entry point and carry the chosen address into the order message. Treat optional contact fields as optional in both the UI and validation.
- Do not pretend a WhatsApp handoff is a completed order. Show the cart total, selected items, fulfillment method, and any price caveat before opening the message; the customer sends it.

## Images and visual direction

- When the owner provides an image, use it to identify the dish and its distinguishing appearance. Do not reuse the same generic food image across unlike products or confuse a roll with a pizza of the same name.
- Follow the established visual system for each category unless the owner asks to change it. Keep new photos coherent in crop, scale, background, and card treatment. If a reference includes unwanted garnish or background, remove or replace those elements in the finished asset.
- A hidden or mystery product can use a deliberate blurred image and question mark, but still needs an accessible name and a clear price.
- Use browsing for current visual references or provider details when the owner requests it. The restaurant's own photos and explicit corrections take precedence over generic web examples.
- Motion should support the brief. If a featured dish carousel should rotate continuously, make the interval and randomization match the owner's request; keep text readable through transitions.

## Changes and publication

- Inspect the existing project before editing. Make focused changes to the source of truth, then verify the rendered page, menu data, image loading, cart behavior, and mobile layout where the change affects them.
- Keep private transcripts, account details, and reusable skills outside the static site's published directory. A private source repository can still expose files through a static host if that host serves its repository root.
- For an authorized deployment, upload the updated source, check the hosting build result, then open the public HTTPS domain and verify the changed content and assets there. A successful build alone does not prove the site works for customers.
- Preserve the existing domain, deployment connection, and unrelated menu data during routine updates. Ask only for information that cannot reasonably be inferred, such as an absent price or an unknown destination for orders.

## Example

[Way Sushi](references/way-sushi-example.md) records the design and product decisions that shaped this skill. It is an example, not a default brand or menu for other restaurants.
