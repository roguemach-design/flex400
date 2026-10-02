# Targeted Flex400 changes — October 2, 2026

Changed site file: index.html. Design, layout, amenities, terms, inquiry form, restrictions, and unrelated copy preserved.

1. Replaced the two location paragraphs with: "Suite B is occupied by Rogue Machine, a precision manufacturing company." Preserved the Rogue Machine name link and its destination. Removed its duplicate address/phone and conflicting call instruction.
2. Replaced every occurrence of "Wheeling WV" with "Wheeling, WV", including the meta description.
3. Added clearly marked INTERIOR_PHOTO_CAPTION_OPTION and caption constants at the top of index.html. Default B preserves the current concept caption; A displays "Suite A interior." The existing caption remains the no-JavaScript fallback.
4. Verified www -> apex HTTP 301. Retained the apex canonical tag on the single page served by both custom and Render hostnames; this is the requested fallback because Render's static rules cannot selectively redirect the onrender hostname.
5. Fixed missing social-image tags: replaced the commented nonexistent photo placeholder with the existing exterior concept WebP in Open Graph and Twitter metadata, added concept image alt tags, and switched Twitter to summary_large_image.
6. Corrected Suite A's structured streetAddress to "400 Public Rd" (unit remains in its name). Added Product alongside Place for the offered suite to satisfy the expected Offer.itemOffered object range. No listing facts changed.

Verification details and exact current values: VERIFICATION-2026-10-02.md. Full extracted JSON-LD: jsonld-current.json.
