# medharborai-website

Source of the MedHarbor website, [medharborai.com](https://medharborai.com).

MedHarbor is an AI medical passport in development: one clear patient card that any doctor can read in their own language. The website explains the idea, the roadmap and how we will protect data, and invites patients, doctors and organisations to join the pilot list.

## Languages

| Folder | Language |
| --- | --- |
| `/` | English |
| `/de/` | Deutsch |
| `/fr/` | Français |
| `/es/` | Español |
| `/ua/` | Українська |

Each language folder has its own `index.html` with its own title, description, canonical link and social preview image. Pages inside each language (Concept, How it works, Impact, Roadmap, For funders, About, Join the pilot and others) are shown with links such as `/#about`.

## Technology

- Plain static HTML, CSS and JavaScript. No framework, no build step, no server code.
- Fonts are self-hosted in `fonts/`. The site makes no requests to third-party servers.
- No cookies and no analytics. The browser's local storage is used only to remember the chosen language and the light or dark theme.
- The pilot form does not send data from the website. It opens the visitor's own email app (or Gmail, if they choose) with a ready message.
- Light and dark themes, and layouts for phones and desktops.

## Structure

```
index.html            English
de/ fr/ es/ ua/       Other languages (index.html in each)
fonts.css, fonts/     Self-hosted fonts
img/                  Photos used on the pages
video/                Explainer video in 5 languages (720p and 1080p) with posters
medharbor-project-brief*.pdf   Project brief (EN, DE, FR)
og-image*.jpg/png     Social preview images
favicon*, icon-*.png, apple-touch-icon.png, site.webmanifest   Icons
robots.txt, sitemap.xml
```

## View it locally

```bash
git clone https://github.com/medharborai/medharborai-website.git
cd medharborai-website
python3 -m http.server 8000
```

Then open <http://localhost:8000> in your browser. Opening `index.html` directly as a file also works, but a local server is closer to how the site runs online.

## Licence

All rights reserved. See [LICENSE](LICENSE). The code, texts, images, videos and documents may not be reused without written permission.

The fonts in `fonts/` (Fraunces, Literata, Figtree, Golos Text and JetBrains Mono) are licensed by their authors under the [SIL Open Font License 1.1](https://openfontlicense.org) and are not covered by the MedHarbor licence.

## Contact

Found a broken link, a typo or a translation mistake? Open an issue or email [info@medharborai.com](mailto:info@medharborai.com).

Security issues: see our [security policy](https://github.com/medharborai/.github/blob/main/SECURITY.md).
