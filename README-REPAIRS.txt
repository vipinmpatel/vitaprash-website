VITAPRASH WEBSITE — REPAIRED STATIC VERSION
===========================================

What was repaired
- Replaced homepage links that pointed to "#" with real internal pages.
- Made the Foundation Bundle button add an £80 bundle to the local browser cart.
- Added checkout.html so the cart no longer leads to a missing page. It clearly states that checkout/payment is not yet available.
- Added privacy.html and terms.html so footer links no longer 404. These are PRE-LAUNCH DRAFTS and must be completed/reviewed before public launch.
- Hardened the shared JavaScript so it does not crash if optional cursor elements or IntersectionObserver are unavailable.
- Removed misleading newsletter/contact success behaviour. The site now clearly says those forms are not connected and that the data has not been sent.
- Added form field names to the contact form to make future service integration easier.

What is still not connected
- Contact form delivery (needs a destination email or form service).
- Newsletter subscriptions (needs a mailing-list service and privacy/consent setup).
- Checkout, payment processing, order confirmation, delivery/tax/returns process.
- Final legal/privacy/terms wording and verified business details.
- Product photos; the supplied ZIP had an empty images folder.

Important
- The cart is browser-only and is not an order system.
- Do not accept payments or orders until a real checkout/payment provider is configured and tested.
- Review the legal draft pages and health/product claims before publishing.
- Keep a backup of the original ZIP.

To deploy on Cloudflare Pages later, upload the CONTENTS of the vitaprash-site folder (so index.html is at the site root), not the outer parent folder.


ARTICLE PUBLISHING (UPDATED)
============================
The Journal and article pages now share js/articles.js as a single article catalogue.
To add an article:
1. Open js/articles.js.
2. Add a new object inside window.VP_ARTICLES. Use a unique id, one of these categories
   (science, ayurveda, transparency), cat_label, title, date, read, excerpt and content.
3. Write content as HTML paragraphs/headings and include direct source links where possible.
4. Save and deploy the site. The Journal listing and related-article links update from the catalogue.
5. Preview on desktop and mobile; verify every source link and claim before publishing.

PRODUCT AND SCIENCE CONTENT
===========================
Product copy has been made more cautious, and the Science page now distinguishes clinical
outcomes from mechanisms and ingredient research. Product details, amounts, prices, testing,
delivery, returns and health claims remain unverified draft data and must be checked against
the final formulation, labels and evidence before launch. Research-search links are discovery
links unless a specific primary paper is linked. The basket/checkout is still not a real
ordering or payment system.
