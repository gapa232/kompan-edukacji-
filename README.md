
# Kompan Edukacji — MVP (PWA)

W pełni działające MVP w formie PWA: profil ucznia (persist w localStorage), TTS/STT (Web Speech API), quiz, notatki, offline (SW), instalacja na Androidzie/iOS (PWA).

## Szybki start (lokalnie)
```bash
npm i
npm run dev
```

## Build i podgląd
```bash
npm run build
npm run preview
```

## Deploy na Vercel
1. Zrób repo na GitHub (np. `kompan-edu-mvp`).
2. Wrzuć pliki repo.
3. Na vercel.com -> New Project -> Import z GitHub -> Framework: Vite -> Build command: `npm run build` -> Output dir: `dist`.
4. Po deployu dostaniesz link w formie `https://twoja-nazwa.vercel.app`.

## Uwagi
- TTS/STT używa Web Speech API (działa w Chrome/Edge/Android; iOS może wymagać interakcji użytkownika).
- Offline: prosty service worker cache-first.
- Dane profilu i notatki są zapisywane w `localStorage`.
- Quiz: przykładowy zestaw 3 pytań (możesz łatwo rozbudować).

## Struktura
- `src/components/TTSSTT.jsx` — mowa (TTS/STT)
- `src/components/ProfileCard.jsx` — profil ucznia
- `src/components/Quiz.jsx` — quiz
- `public/sw.js` — service worker
- `public/manifest.webmanifest` — PWA manifest

---
Autor projektu: **Krzysztof Gapski**
