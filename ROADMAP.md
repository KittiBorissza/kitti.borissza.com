# Roadmap: kitti.borissza.com

Written 19 Nov 2026. This file is the place to resume. The site is a personal portfolio, built in small phases so a later run can continue without starting over.

## How to resume

1. Find the first phase below that is not **Done**, and do the next unchecked task.
2. The approved brief is not in this repo. It lives in Kitti's Google Drive as the PO_Brief doc. Use that for structure and for any wording. Public page copy is Appendix A of the brief. Do not add claims, numbers, clients, or testimonials that are not in that copy.
3. Homepage directions are in [drafts/](drafts/index.html). Draft D is the proposed hybrid of A and C, pending Kitti's sign-off. Do not build the real pages until she signs off.
4. Images already in the repo: `images/Portre-06_Borissza_Kitti.jpg` (credit: Photo: Németh András Péter) and `images/linkedin_header.jpg` (her woven roots-and-leaves artwork, decorative). The Compass stage photo and the Hacker Paradise photo are not in the repo. Use a labelled placeholder until Phase 6 clears them.
5. Update the status of any phase you work on before stopping, including when a run ends early.

**You are here:** Draft D is the proposed direction, pending Kitti's sign-off. Next is that sign-off (Phase 2), then the build.

---

## Phase 0 — Brief approved

**Status:** Done

- [x] Brief approved on 19 Nov 2026, including positioning and the portfolio objective
- [x] Page copy treated as final (Appendix A of the brief)
- [x] Brief kept in Kitti's Google Drive PO_Brief doc, not in this repo

**Definition of done:** The brief is the source of truth for copy, structure, and what is allowed on the site. Met.

## Phase 1 — Design drafts

**Status:** Done

- [x] `drafts/a/`, `drafts/b/`, and `drafts/c/`: three single-file homepage drafts (HTML and CSS only)
- [x] `drafts/index.html` with a one-line description of each
- [x] Same approved copy and section order in each draft; different layout
- [x] Desktop (1440) and mobile (390) screenshots for review, attached to the pull request, not stored in the repo
- [x] `drafts/d/`: hybrid of A (paper hero, portrait, woven band, main CTA) and C (three dark door panels, then square cards on the paper). Proposed direction, pending Kitti's sign-off

**Definition of done:** Kitti can open the drafts and compare them. Draft D is the proposed direction, pending her sign-off. The rest of the site is not built. Met.

## Phase 2 — Kitti picks a direction

**Status:** In progress. She likes A and C and approved a hybrid. Draft D is that hybrid, pending her sign-off.

- [x] Review drafts A, B, and C on a desktop and a phone
- [x] Choose one direction, or name the parts to combine: A’s top, C’s three door panels, square cards on the paper below
- [ ] Kitti signs off on draft D
- [ ] Note any copy changes or crop changes before build

**Definition of done:** A written choice of direction, including any mix of parts, so the build does not have to guess. Sign-off on D meets this.

## Phase 3 — Tech setup

**Status:** Not started

Recommendation, cheapest simple path:

- **Stack:** Astro, output as a static site, with the copy in Markdown so a Hungarian locale can reuse the same structure later. Plain HTML and CSS is the fallback if a build step is not worth it; the drafts already show that the homepage can be done that way.
- **Hosting:** GitHub Pages is the simplest, because the repo is already on GitHub. Netlify or Vercel are fine alternatives if preview deploys are wanted. No server.
- **Domain:** DNS for kitti.borissza.com is still to be confirmed. Build and review can happen on a host preview URL before the domain is pointed.

- [ ] Confirm the stack (Astro, unless plain HTML is chosen instead)
- [ ] Confirm the host
- [ ] Write down who controls DNS for kitti.borissza.com, and point it only when the preview looks right
- [ ] Add the page shell: header, footer, skip link, focus, contrast, `lang="en"`
- [ ] Put copy in Markdown (or HTML files, if that was the choice) so it can be checked against the brief

**Definition of done:** One real page deploys to a preview URL, and the domain plan is written down even if DNS is not switched yet.

## Phase 4 — Build pages

**Status:** Not started

Build from the chosen draft. Keep the homepage order: hero (headline, intro, main CTA, roots-and-leaves band), three equal doors, featured work, Campaigns for causes, Now strip, browse-the-work chips, the "Who we build with shapes what we build" band, contact, footer.

- [ ] Home
- [ ] Work: three featured case studies, then Earlier work with role-type filters
- [ ] Filters use a URL parameter, and the full tagged list still shows with no JavaScript
- [ ] Case study: WAC / We Are Museums
- [ ] Case study: Climate Game On
- [ ] Case study: EasyA × Tezos Hackathon, London
- [ ] About
- [ ] Work together, with the consultation booking control omitted
- [ ] Contact via the header, the homepage, Work together, and the footer (no separate contact page)
- [ ] Main CTA opens an email to kitti@borissza.com with the subject "Hello from kitti.borissza.com"
- [ ] 404 page

**Definition of done:** Every page in the site map uses the brief's copy and the chosen visual direction. A filtered Work link can be shared, and the list still makes sense with JavaScript off.

## Phase 5 — Content and image QA

**Status:** Not started

- [ ] Check every page against the brief's copy. Remove anything that was not in it
- [ ] Portrait crop: lamp out of frame, not tighter than her hands, credit "Photo: Németh András Péter", alt "Kitti Borissza smiling at a desk."
- [ ] Woven header is decorative (empty alt). Swap in the hi-res original when Phase 6 has it
- [ ] Compass stage slot and Hacker Paradise slot stay labelled placeholders until Phase 6
- [ ] One leaf-green accent, used for the main CTA and at most one highlighted word in a section. Not as small text on the off-white background
- [ ] Contrast, focus, heading order, and tap targets (at least 44px)
- [ ] No prices, and no booking button

**Definition of done:** A pass against the brief, plus a short list of assets still waiting on Phase 6.

## Phase 6 — Pre-publication checklist

**Status:** Not started

- [ ] CraftHub written OK for the stage photo. Use only the approved crop, credited "Photo: CraftHub"
- [ ] Consent of identifiable people in any photo that shows them, or crop so they are not identifiable
- [ ] LinkedIn header: hi-res original supplied, and reuse rights confirmed
- [ ] Kitti approves the portrait crops
- [ ] Booking link stays optional and hidden until Kitti provides one. No prices on that page either
- [ ] Case studies launch without external source links. Add a Sources strip only when real URLs are ready

**Definition of done:** Each item is checked or explicitly deferred, and nothing still waiting on permission is on the live site.

## Phase 7 — Launch

**Status:** Not started

- [ ] Kitti reviews the preview
- [ ] DNS for kitti.borissza.com points at the host, over HTTPS
- [ ] Smoke-check Home, Work, a filtered Work link, one case study, About, and Work together
- [ ] The main CTA opens an email with the subject "Hello from kitti.borissza.com"

**Definition of done:** kitti.borissza.com serves the site over HTTPS and those paths work.

## Phase 8 — Post-launch

**Status:** Not started

- [ ] Update the Now strip after 25 Nov 2026
- [ ] Update the Now strip after December 2026
- [ ] Update the Now strip after January 2027
- [ ] Move finished Now items to "Recently" or to Earlier work. Do not add a Now item that is not in the brief
- [ ] Hungarian localisation later, same structure, `lang="hu"`

**Definition of done:** The Now strip matches what is actually current at each of those dates, and Hungarian is either scheduled or shipped.
