# Admin Dashboard (React + Vite + Tailwind)

A dark-themed e-commerce admin dashboard built with React, Vite and Tailwind
CSS. It has seven pages of stat cards, charts and tables with Framer Motion
entrance animations. All figures come from static mock data inside the
components; there is no backend.

> Despite the repository name, this project is React only. It does not use Vue.

## Pages

| Route | Contents |
| --- | --- |
| `/` | Overview: stat cards, sales overview line chart, category distribution pie, sales-by-channel bar chart |
| `/products` | Product stats, searchable products table, sales trend chart |
| `/users` | User stats, searchable users table, user growth, activity heat map, demographics |
| `/sales` | Sales overview, sales by category, daily sales trend |
| `/orders` | Order stats, daily orders chart, order status distribution, searchable orders table |
| `/analytics` | Revenue vs target, channel performance, product performance, retention, customer segmentation radar, a static "insights" panel |
| `/settings` | Profile, notifications toggles, security, connected accounts, danger zone (UI only) |

## Tech stack

- React 19 + Vite 6
- Tailwind CSS 3 (via PostCSS)
- Recharts for all charts
- Framer Motion for animations
- `lucide-react` icons
- React Router 7 for navigation; a collapsible animated sidebar

## Project layout

```
src/
  App.jsx                 routes
  pages/                  one component per page
  components/common/      Sidebar, Header, StatCard
  components/<section>/   charts and tables for each page
```

## Running locally

Requires Node.js.

```bash
npm install
npm run dev
```

Other scripts: `npm run build` (production build to `dist/`), `npm run preview`,
`npm run lint`.
