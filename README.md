# HarEvent Event Planner

Responsive React + Vite + Tailwind implementation based on the supplied master prompt.

## Run locally
1. Install Node.js (LTS).
2. Extract the ZIP and open this folder in VS Code.
3. Open a terminal in this folder and run:
   ```bash
   npm install
   npm run dev
   ```
4. Open the local URL printed by Vite (usually http://localhost:5173).

## Build for deployment
```bash
npm run build
npm run preview
```

## Notes
- Images use remote Unsplash image URLs as visual placeholders. Replace them with licensed assets exported from Figma or your own `public/images` files for an exact match.
- The provided prompt references an uploaded HarEvent logo (Image 9), but that image was not included as an accessible image asset in the text attachment. The header/footer therefore use a simple text-based temporary mark; replace it with the original logo file when available.
- The filter chips and wishlist hearts are interactive. Navigation links scroll to page sections. Inquiry/login/chat controls are front-end placeholders and do not submit to a backend.


## Latest requested updates
- Removed star ratings and review counts from planner cards; location remains visible.
- Kept featured planner category filters left-aligned.
- Standardized typography: Poppins for interface/body, Playfair Display for hero/About serif headings, Dancing Script for the detail note.
- Replaced unsupported social-media brand icon imports with supported Lucide icons to avoid Vite import errors.
- Replaced `ChartNoAxesCombined` with `BarChart3`.

## Vercel deployment
1. Push this project to GitHub.
2. Import the repository in Vercel.
3. Select Vite, use `npm run build` as the build command, and `dist` as the output directory.
