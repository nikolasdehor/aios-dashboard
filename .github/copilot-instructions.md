# Copilot Instructions — aios-dashboard

## Project Overview
aios-dashboard é uma aplicação Next.js (App Router) com TypeScript para dashboard do sistema AIOX.

## Stack
- **Next.js 14+** com App Router
- **React 18+** + TypeScript estrito
- **TailwindCSS** quando aplicável
- Server vs Client Components separados conscientemente

## Conventions
- Server Components por padrão; `'use client'` só onde necessita state/effects/browser API
- Tipagem explícita; sem `any` implícito
- Metadata exports pra SEO em páginas relevantes
- Server Actions com validação de input
- Variáveis sensíveis via env (`NEXT_PUBLIC_` só pro que é público mesmo)
- Sem `console.log` em produção

## Folder Structure
- `app/` — rotas, layouts, pages
- `components/` — componentes (.tsx)
- `lib/` — utilitários, clientes
- `public/` — assets estáticos

## Development
- `pnpm install`
- `pnpm dev`
- `pnpm build` + `pnpm start`
- `pnpm lint`

## Critical Files
- `app/layout.tsx` — root layout
- `app/page.tsx` — home
- `next.config.{js,mjs}` — config Next
- `package.json`
