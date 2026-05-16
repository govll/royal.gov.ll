# Royal Household of Links Land — royal.govll.org

## File structure

```
/
├── index.html                  ← Home page
├── monarchy/
│   └── index.html              ← /monarchy
├── constitution/
│   └── index.html              ← /constitution
├── succession/
│   └── index.html              ← /succession
├── honours/
│   └── index.html              ← /honours
└── assets/
    ├── style.css               ← Shared stylesheet (all pages link to /assets/style.css)
    └── links-land-flag.png     ← DROP YOUR FLAG IMAGE IN HERE
```

## Before deploying

1. Place your flag image at `assets/links-land-flag.png`
   - It appears in the masthead (44×44px) and as the panel image (120×120px)
   - PNG with transparent background works best

2. All internal links use root-relative paths (e.g. `/monarchy`, `/assets/style.css`)
   so the site must be served from the root of the `royal.govll.org` domain.

3. Your server needs to serve `index.html` for clean URLs like `/monarchy`
   (most static hosts — Netlify, Vercel, GitHub Pages, Apache, Nginx — do this automatically).

## Pages

| URL              | File                        | Purpose                          |
|------------------|-----------------------------|----------------------------------|
| /                | index.html                  | Home / overview                  |
| /monarchy        | monarchy/index.html         | About the Monarch & royal duties |
| /constitution    | constitution/index.html     | Constitutional powers (Art. 4-6) |
| /succession      | succession/index.html       | Succession rules (Art. 5)        |
| /honours         | honours/index.html          | Royal honours & titles           |

## Styling

All pages share `/assets/style.css`. The design matches the govll.org aesthetic:
- Colours: maroon (#571626), navy (#07196d), gold (#b17922)
- Fonts: Georgia (headings), Arial (body) — system fonts, no CDN required
- Top strip: maroon / gold / navy tricolour
- Fully responsive down to 460px
