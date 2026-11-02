# Lisa Liu — Portfolio v1

A responsive editorial portfolio built with Next.js App Router, TypeScript, React and CSS. Ready for Vercel.

## Run locally

```bash
npm install
npm run dev
```

Open http://localhost:3000.

## Deploy to Vercel

1. Upload this folder to a new GitHub repository.
2. In Vercel, choose **Add New → Project → Import Git Repository**.
3. Keep framework preset **Next.js**, then select **Deploy**.
4. Review the preview URL before pointing a custom domain to it.

## Important before publishing

- **Artwork:** Project images currently reference original publicly hosted Framer assets (external URLs). These are real artwork, not AI-generated placeholders. For reliability, export/download originals into `/public/projects/` when possible and update `lib/projects.ts` to local paths. External images require the original Framer assets to remain publicly available.
- **Case studies:** The seven included project descriptions are condensed from the original public portfolio. Original case study links are preserved on each page. Verify the client/concept designation for Walmart and the accuracy of each description before publication.
- **Contact:** The contact CTA intentionally links to the original portfolio contact section; replace with your verified email or contact form before publishing. No email address was invented.
- **More original projects:** Shiru’s Resort, Flowever Floral and Earth Writing appear in the original portfolio but are not yet migrated in this first version.
- **Permissions:** Confirm permission to publish any client work and any third-party brand artwork.
- **No production deployment has been performed.**

## Structure

- `app/page.tsx` — Home / selected work / about / contact
- `app/projects/[slug]/page.tsx` — dynamic case studies
- `lib/projects.ts` — project content and images
- `app/globals.css` — editorial design system and responsive layout
- `components/` — header and project cards

## Design tokens

- Ivory `#F8F5EF`
- Beige `#EAE2D6`
- Espresso `#352E29`
- Accent `#A7795E`
