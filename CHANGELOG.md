# Changelog

[Русская версия](CHANGELOG_ru.md)

## 2026-10-03

- Adopted a single naming standard for docs across Trio, Peel and
  Monologue: English `README.md` / `CHANGELOG.md`, Russian
  `README_ru.md` / `CHANGELOG_ru.md`, with a one-line language switch
  at the top of each (after the licence badge, where there is one).
- Fixed the licence badge and the "Licence" section to use British
  spelling throughout (`licence` as the noun); the file itself stays
  named `LICENSE`, unchanged.
- Audited `index.html`, `peel.html`, `monologue.html` and `cover.html`
  for stray Russian developer comments in CSS/JS. Found none — every
  Cyrillic line in all four files is an interface string inside the
  RU/EN translation tables, which is correct as-is and was left
  untouched.
