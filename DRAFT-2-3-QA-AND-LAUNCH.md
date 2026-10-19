# Makonde Draft 2.3 — Launch Candidate QA

Date: 19 October 2026

## Automated checks — PASS
- 14 HTML files inspected; 13 content pages (404 excluded from H1 check).
- Shared stylesheet consistent on all content pages.
- Local HTML, image, script and stylesheet references: no missing files.
- JSON-LD structured data: valid on inspected pages.
- Exactly one H1 on each content page.
- FormSubmit AJAX endpoint, consent and form validation remain in place.
- CSS consolidated by removing 193 redundant declarations with identical selectors and at-rule scopes; cascade order retained.
- Skip-navigation and Escape-to-close mobile navigation added.

## Not verified — mandatory launch gates
- Browser rendering on real desktop/mobile viewports; no Playwright browser run completed.
- WCAG keyboard and screen-reader manual audit, automated Lighthouse accessibility/performance scores.
- Live FormSubmit activation, CAPTCHA behavior, delivery and mailbox receipt.
- DNS/SSL/redirect behavior of www.makondeinvest.co.za and indexing in Search Console.
- OEM partnership claims, content, image licensing, and legal/POPIA approvals.
- Independent malware/antivirus scan of deployable files.

## Production handover
1. Deploy this entire folder's contents (not the enclosing folder) to staging; remove any obsolete files such as assets/layout-v13.css.
2. Test every navigation route and mobile menu at 360, 390, 768, 1024, 1440 and 1920px, and browser zoom at 100% and 200%.
3. Have Elaine activate FormSubmit. Submit a real test enquiry, confirm it arrives, and verify spam handling and reply-to.
4. Obtain written approval for copy, partnership descriptions, photographs, legal terms and privacy notice.
5. Confirm DNS, HTTPS, preferred www redirect, sitemap, canonical URLs, robots directives and Search Console on production.
6. Remove the draft notice only after approvals. Do not publish this build as a final approved production site until these gates pass.

## Notes
The live GitHub Pages URL is a preview; the site's canonical and sitemap addresses point to www.makondeinvest.co.za. Staging should not be independently indexed.
