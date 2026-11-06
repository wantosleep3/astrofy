# Eris — Personal Portfolio

Personal portfolio for **Eris**, focused on electronics, component data, digital products, AI-assisted workflows, and small software experiments.

**Live site:** https://werwerwer.eu.org/

## Featured work

- **[AI BOM Copilot](https://werwerwer.eu.org/projects/ai-bom-copilot/)** — a personal prototype exploring BOM normalization and component candidate search. The demo runs separately on Cloudflare Workers.
- **[Component Parameter Architecture](https://werwerwer.eu.org/projects/component-data-architecture/)** — an anonymized work case study on component attribute standardization, category mapping, and data quality.
- **[Component Search Experience Redesign](https://werwerwer.eu.org/projects/search-experience/)** — an anonymized work case study on search-result usability, filter behavior, and funnel measurement.

Work case studies intentionally omit company-confidential systems, customer information, internal files, and proprietary datasets. Project descriptions distinguish personal prototypes from work contributions and state known demo limitations.

## Tech stack

- [Astro](https://astro.build/)
- [Tailwind CSS](https://tailwindcss.com/)
- [DaisyUI](https://daisyui.com/)
- JavaScript / TypeScript
- Cloudflare Workers for the standalone AI BOM Copilot demo

## Local development

Install dependencies:

```bash
pnpm install
```

Start the development server:

```bash
pnpm dev
```

Build the static site:

```bash
pnpm build
```

## Project structure

```
src/
├── components/       # Shared UI and CV components
├── content/          # Astro content collections
├── layouts/          # Shared page layouts
└── pages/
    ├── projects.astro
    ├── projects/     # Individual project case studies
    ├── cv.astro
    └── index.astro
public/               # Static assets
```

## Deployment notes

The portfolio site and the AI BOM Copilot demo are deployed independently. The project detail page links to the Worker demo; it does not proxy or embed the Worker application under the portfolio domain.

## Template attribution and license

This site was originally built from [Astrofy](https://github.com/manuelernestog/astrofy), an open-source Astro portfolio template by [Manuel Ernesto](https://github.com/manuelernestog). The original template is licensed under the [MIT License](https://github.com/manuelernestog/astrofy/blob/main/LICENSE). This repository retains the original template's license and attribution.
