# Flex400 revision

## Removed or merged
- Removed extra navigation links and repeated leasing/contact copy; retained one hero CTA and one sticky header CTA.
- Replaced eight feature cards and filler descriptions with a compact two-column spec list. All eight specifications remain.
- Consolidated location into address, access sentence, nearby markets, and directions link.
- Replaced the conceptual rendering with a labeled real-photo slot to avoid depicting an unverified interior.
- Reduced inquiry fields to Name, Email or mobile, Intended use, and Desired move-in date. Restrictions sit immediately above the buttons.
- Removed repeated footer contact information. Retained owner attribution.
- Removed heavyweight embedded conceptual imagery and unnecessary styling. Compressed the supplied wordmark to WebP; critical CSS stays inline, with no dependencies, web fonts, map iframe, or server.

## SEO and behavior
One H1, logical H2s, a 47-character title, 155-character description, robots.txt, sitemap.xml, favicon, canonical and social metadata. JSON-LD describes the listing, monthly offer, address and approximate floor area. All required nearby markets appear once in visible copy. Public email is omitted; the draft destination is reconstructed in JavaScript. This discourages basic scrapers but is not strong protection.

The fully static form opens an email or text draft. The visitor must send it; the page does not collect or transmit submissions to a server. Calls remain by appointment only.

## Owner placeholders
- Verify drive times to Wheeling WV and I-70; the source contains a hidden marker. Public copy currently claims no travel time.
- Verify property latitude/longitude before adding GeoCoordinates. Source comment shows where to add them; invalid placeholder coordinates are omitted from published JSON-LD.
- Supply real Suite A interior photographs and a social image. Suggested paths: assets/suite-a-interior.avif, assets/suite-a-interior.webp, assets/suite-a-social.webp. Include explicit dimensions, descriptive alt text and lazy loading for interior photos. Enable the staged social image tags only once the image exists.
- Optional: supply a licensed static location map and required attribution after coordinates are verified. Currently directions link only, with no fictitious map.
- Connect/confirm https://flex400.com/; then replace the Render origin in canonical, og:url, structured-data identifiers, robots.txt and sitemap.xml. Current canonical correctly points to the live Render site.
- Confirm the existing inquiry email destination, roguemach@gmail.com, or supply its replacement. It is not shown in body copy.

## Verification
Visible body word count: 386 before, 204 after (47.2% reduction). Method excludes metadata, scripts, styles, comments and hidden placeholders. Original HTML: 2,000,183 bytes; revised HTML approximately 20 KB (99% reduction). All eight specs and exact restriction meaning retained. One H1, description length, JSON parsing, once-only key facts/market mentions and JavaScript syntax checked.

Lighthouse: not run; no installed Lighthouse/browser audit runtime was available. Scores of 95+ are a target, not a measured result. Run mobile Lighthouse after deploying and again after adding photos. No invented before/after scores.

## Deployment
Static root files: index.html, robots.txt, sitemap.xml, render.yaml. No build step or application server required. Current host: https://flex400.onrender.com/. Source: https://github.com/roguemach-design/flex400.
