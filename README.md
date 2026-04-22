# raklane.github.io

Personal portfolio site for Rakesh Kumar — Lead SDET at Snap Inc.

Live at **https://raklane.github.io**

## Structure

```
.
├── index.html                       Single-file site (HTML + CSS + JS inline)
├── .nojekyll                        Disable Jekyll processing on GitHub Pages
├── README.md
└── assets/
    ├── rakesh.jpg                   Profile photo
    ├── files/
    │   └── RakeshKumar_Resume.pdf   Latest resume
    └── project/
        ├── api_db_framework.png
        ├── cricpredict.gif
        └── genai.webp
```

Everything is inline in `index.html` — no build step, no external CSS/JS beyond Google Fonts and the Google Analytics tag.

## Deploy

Push to the `main` branch of the `raklane.github.io` repo. GitHub Pages serves it automatically.

## Analytics

The site reports to Google Analytics 4 property `G-FDQ7DR8FVQ` and emits these custom events:

| Event | When it fires |
| --- | --- |
| `scroll_depth` | Visitor crosses 25 / 50 / 75 / 100 % of page height |
| `section_view` | A section first becomes visible |
| `section_dwell` | A section leaves the viewport (payload: seconds spent) |
| `outbound_click` | Click on any external link |
| `email_click` | Click on any `mailto:` link |
| `resume_download` | Click on the resume PDF |
| `anchor_click` | In-page nav click |
| `mobile_menu_toggle` | Hamburger opens / closes |
| `experience_tab_switch` | User switches company tab |
| `page_exit` | `beforeunload` — total engagement time in seconds |

View them in GA4 under *Reports → Engagement → Events* (live data shows up in *Realtime* within ~30 seconds).

## Updating the resume

Replace `assets/files/RakeshKumar_Resume.pdf` with the new file and commit. All three resume links in the site point at this single file.
