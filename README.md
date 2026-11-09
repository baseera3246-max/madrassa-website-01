# Madrassa Aysha Siddiqa Lilbanat Katlang: website

React + TypeScript + Vite + Tailwind CSS + lucide-react. Languages: English (LTR), Urdu and Arabic (RTL).

## Run
    npm install
    npm run dev        # local
    npm run build      # type-check + production build into dist/

## Edit content
- All text (EN/UR/AR): `src/i18n.ts`. Program names are `P` (UR/AR) and `PROGRAMS_EN`.
- WhatsApp number: `VITE_WHATSAPP_NUMBER` (copy `.env.example` to `.env`). The default is a dummy.
- Colours/typography: `src/index.css` and `tailwind.config.js`.

## Before publishing (placeholders to confirm)
Programs offered, "why choose us" claims, vision/mission, principal name/photo/message, real photos in the gallery
(`GalleryArt` in `src/components/ui.tsx` is placeholder art), WhatsApp number, Google Maps embed, social links, domain in SEO tags.

## Inquiry forms
`src/lib/inquiries.ts` is the single backend hook. It currently returns `false`, so the UI says nothing was sent.
Add Firebase there (instructions in the file) and the forms will report success automatically.

## Deploy to Vercel (not done yet)
Import the repo in Vercel (framework: Vite), add the env vars, deploy. `vercel.json` is already included.
