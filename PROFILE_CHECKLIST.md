# GitHub profile upgrade checklist

## Publish the profile README

1. On GitHub, create a **public** repository named exactly `maninderjit-johar`.
2. Do not initialize it with another README if you plan to push this folder.
3. Push `README.md` from this folder to the repository's default branch.

## Profile settings

- Name: `Maninderjit Johar`
- Suggested bio: `Full-Stack Developer | React · TypeScript · Node.js | Building polished, reliable web products`
- Location: `Mississauga, Ontario, Canada`
- Website: `https://portfolio-maninderjit-johars-projects.vercel.app`
- LinkedIn: `https://www.linkedin.com/in/manijohar`
- Turn on **Include private contributions on my profile** under Profile settings if you want private work represented as anonymized contribution squares.

## Repair missing contribution attribution

GitHub credits commits only when the commit email is attached to your account and the commits land on the repository's default branch (or `gh-pages`). Add `maninderjit.johar@outlook.com` to GitHub under **Settings → Emails**, then verify it.

Configure future commits:

```bash
git config --global user.name "Maninderjit Johar"
git config --global user.email "maninderjit.johar@outlook.com"
git config --global user.useConfigOnly true
```

Check the identity used in an existing repository:

```bash
git log --format='%h  %an  <%ae>' --all | sort -u
```

If old commits use another email that you own, the safest fix is usually to add and verify that email on GitHub. Avoid rewriting published history solely to color the graph: it changes commit IDs and can disrupt collaborators.

## Pin these repositories

Pin in this order:

1. `cinequiz`
2. `essentialui`
3. `aspirearc`
4. `portfolio`

Leave `hypercare-challenge` unpinned unless its generic Create React App README is replaced with a project-specific case study.

## Repository presentation upgrades

For every pinned repository, add:

- a one-sentence outcome-focused description;
- a live demo URL when available;
- 5–8 relevant repository topics;
- a screenshot or short GIF near the top of the README;
- clear features, stack, local setup, architecture decisions, and future improvements;
- a license if you want others to reuse the code;
- passing build/test/lint automation where appropriate.

Suggested descriptions and topics:

| Repository | Description | Topics |
|---|---|---|
| `cinequiz` | `Interactive movie quiz built with React, TypeScript, Vite, and Tailwind CSS.` | `react`, `typescript`, `vite`, `tailwindcss`, `quiz-app`, `frontend` |
| `essentialui` | `Lightweight, responsive, and themeable sidebar component for React applications.` | `react`, `javascript`, `component-library`, `sidebar`, `responsive-design`, `ui` |
| `aspirearc` | `Full-stack fitness logging application built with Next.js and Prisma.` | `nextjs`, `prisma`, `typescript`, `fitness`, `full-stack`, `react` |
| `portfolio` | `Personal developer portfolio built with Astro and Tailwind CSS.` | `astro`, `tailwindcss`, `portfolio`, `responsive-design`, `frontend` |

## Achievements and activity

Your profile already displays Quickdraw ×2 and YOLO ×2. GitHub achievements should be earned through genuine collaboration; do not manufacture activity or low-value pull requests for badges.

A stronger long-term signal is consistent, meaningful work:

- ship improvements to the pinned projects through focused pull requests;
- contribute useful fixes or documentation to projects you actually use;
- open well-researched issues with reproductions;
- review collaborators' pull requests;
- publish tagged releases and concise changelogs for reusable projects.

