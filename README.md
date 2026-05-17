# VSWear Website

Public-facing recruitment website for the **VSWear** clinical research study — an Oxford-led wearable technology study for people with Vestibular Schwannomas.

Live site: [https://shay-dt.github.io/VS_Wear_website/](https://shay-dt.github.io/VS_Wear_website/)

---

## About the study

VSWear is an Oxford University Hospitals NHS Foundation Trust research study investigating wearable-derived measures of balance and dizziness in people with Vestibular Schwannomas. The study aims to:
- Improve early detection of balance problems
- Explore new treatment options

**Ethics reference:** MS IDREC 1000079

---

## Tech stack

- [Hugo](https://gohugo.io/) — static site generator
- Theme: `theme-long-teng` (submodule)
- Deployed via GitHub Actions to GitHub Pages

---

## Project structure

```
content/          # Page content (editable Markdown files)
  _index.md
  product.md      # Hero banner text
  nav.md          # Navigation bar links
  user-trust.md   # Stats/trust section
  how-to.md       # How to get involved steps
  team.md         # Team member details
  footer.md       # Footer text and links

layouts/          # Hugo templates (override theme defaults)
  _default/
    baseof.html   # Base HTML shell
  index.html      # Homepage layout
  partials/
    navbar.html   # Navigation bar
    footer.html   # Footer

static/
  css/
    custom.css    # All custom styles
  img/            # Logos and team photos
  poster.pdf      # Study poster
  PIS.pdf         # Participant information sheet

themes/
  theme-long-teng/  # Base theme (git submodule)
```

---

## Running locally

Requires [Hugo](https://gohugo.io/installation/) to be installed.

```bash
hugo server -D
```

Then open [http://localhost:1313](http://localhost:1313).

---

## Deploying

Deployment is automatic. Any push to the `main` branch triggers a GitHub Actions workflow that builds the Hugo site and publishes it to GitHub Pages.

To update content, edit the relevant file in `content/` and push.

---

## Team

| Name | Role |
|------|------|
| Sanjeeva Jeyaretna | Principal Investigator — Consultant Neurosurgeon, Oxford |
| Aiden Doherty | Principal Investigator — Professor of Biomedical Informatics, Oxford |
| Chrystalina Antoniades | Principal Investigator — Professor of Clinical Neuroscience, Oxford |
| Shay Sivanathan | Lead Researcher — Clinical Research Fellow, Oxford |

---

## Contact

Email: [shay.sivanathan@ouh.nhs.uk](mailto:shay.sivanathan@ouh.nhs.uk)
