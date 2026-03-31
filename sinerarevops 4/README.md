# sinerarevops.com

## Repo structure

```
/
├── index.html                          ← English landing page (live at sinerarevops.com)
├── vercel.json                         ← Clean URL routing
├── assets/
│   └── images/
│       ├── SINERA_REVOPS_polished.png  ← Logo (navbar)
│       ├── Pipeline_Engine2.png        ← Hero visual
│       ├── sinera_hero_visual_v4.png   ← How It Works diagram
│       ├── og-image.png                ← Social share image (1200×630px)
│       └── favicon.png                 ← Browser tab icon
└── tr/
    └── index.html                      ← Turkish version (add when ready → sinerarevops.com/tr)
```

## Image upload checklist

Before going live, upload these files to /assets/images/ in the repo:

- [ ] SINERA_REVOPS_polished.png
- [ ] Pipeline_Engine2.png
- [ ] sinera_hero_visual_v4.png
- [ ] og-image.png (create a 1200×630px version of the logo/hero for LinkedIn previews)
- [ ] favicon.png (32×32px or 64×64px version of the logo mark)

## Deployment

1. Push this repo to GitHub
2. Connect to Vercel → import repo → deploy
3. Add domain sinerarevops.com in Vercel project settings
4. Point DNS at registrar:
   - A record: @ → 76.76.21.21
   - CNAME: www → cname.vercel-dns.com

## Adding Turkish version

1. Create /tr/index.html (copy index.html, translate all text)
2. In index.html: uncomment .lang-switcher (set display: block)
3. In tr/index.html: add matching lang switcher pointing back to /
4. Push → Vercel auto-deploys

## Contact email

hello@sinerarevops.com → configure as alias in M365 Admin Centre
