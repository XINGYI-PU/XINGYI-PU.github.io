# Xingyi Pu — Academic Homepage

This repository contains Xingyi Pu's academic homepage, built with [al-folio](https://github.com/alshedivat/al-folio).

The content is based on the supplied CV, project repositories, and [LinkedIn profile](https://www.linkedin.com/in/xingyipu/), with a focus on AI, IoT, connected devices, and intelligent mobility. See the [LinkedIn sync notes](docs/LINKEDIN_SYNC.md) for the verified September 18, 2026 snapshot.

The design takes inspiration from [Huangxun Chen's profile sidebar and research-first homepage](https://www.chenhuangxun.com/) and [Seong Jae Hwang's restrained typography and dated academic record](https://sites.google.com/yonsei.ac.kr/micv/seongjae). The homepage brings together a personal profile, research interests, selected projects, education, awards, and experience.

## Updating the site

- Edit the biography and academic record in `_pages/about.md`.
- Add or edit projects in `_projects/`; the homepage displays the first three by `importance`, and the projects page lists all of them.
- Update contact links in `_data/socials.yml` and the full CV in `_data/cv.yml`.
- The CV is temporarily unpublished: its page, data, PDF, and local publishing outputs are excluded from the public repository by `.gitignore`, and the RenderCV workflow is disabled. The local page has `nav: false` and `published: false`, and `_config.yml` excludes its PDF. To publish the CV later, review its personal information, update these exclusions and flags, and rebuild. The source page, CV data, and PDF remain available locally for editing.
- Research, Projects, Publications, and individual project pages remain published. Homepage links to these pages are controlled by `detail_pages_enabled` in `_pages/about.md`.
- The personal design lives in `assets/_sass/_academic.scss`, the directory used by the theme's stylesheet cache key. The `assets/css/main.scss` override preserves the core gem imports and loads this partial last. This personal-site override is tracked by `.al-folio-overrides.yml`; see the [override maintenance workflow](docs/ARCHITECTURE.md#local-overrides-your-site-vs-this-repo) when upgrading the core gem.

## Local development

```bash
bundle install
npm ci
bundle exec jekyll serve
```

Then open `http://localhost:4000/`.

This is a user homepage for `xingyi-pu.github.io`, so `_config.yml` intentionally keeps `baseurl` empty. Build with `bundle exec jekyll build` without the starter's `/al-folio` prefix.
