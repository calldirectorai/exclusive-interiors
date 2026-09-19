# exclusive-interiors.com

Static site: `index.html` + `images/` (WebP). No build step. Deploy the folder as-is.

## Before go-live (search index.html for "TODO" / "REPLACE_")
1. **Contact form** - set `FORM_ENDPOINT` (top of the main script) to the intake flow
   webhook in the new app.calldirector.ai account. Until then the form shows a
   "not connected" message instead of pretending to send. Payload is JSON:
   full_name, email, phone, project_type, budget, message, source, submitted_at.
2. **Chat widget** - the old PayMeGPT embed is commented out at the bottom of
   index.html. Paste the new account's embed there.
3. **SEO tags** - copied from the live site. The live meta description was cut off
   in the copy that was read ("...high-end in"); it is completed here as
   "high-end interiors". The live title ends in "& Custom"; confirm both.
   `og:image` points at images/grand-hall-ceiling.webp.
4. **Testimonials and stats band** - placeholders. Replace with verified client quotes
   and real numbers before launch.

## Images
- `images/` holds every image the page uses (20 files, ~2.2 MB total).
- `images/extra/` holds unused photos kept for future gallery additions.
- Source screenshots from Dec 7 2025 carried browser UI overlays; edges were trimmed.
  Replace with original camera files when available.
- Pool-framing close-ups are crops of one collage (the only pool-framing photo on hand).

## Ownership checklist for cutover
- Confirm who controls the exclusive-interiors.com registrar login and DNS.
- Deploy to a preview URL first; test images, form, phone links, chat widget.
- Switch DNS last; leave the old setup untouched for a few days.
