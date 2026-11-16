# Aften-sync – planlagt opgave

Hver af os har en planlagt opgave, der kører hver aften. Den oprettes på claude.ai/code/routines (New task → Set up manually). Under Advanced settings → Repository vælges dide0001/Headspace_md. Kopiér teksten nedenfor ind som instruktioner, og skift NAVN/navn og ANDEN/anden ud (fx Aviaja/aviaja og Diego/diego).

---
Du er NAVNs assistent i eksamensprojektet for headspace. Repoet Headspace_md er NAVN og ANDENs fælles hukommelse for deres to Claude'er. Arbejd altid direkte på branchen main (ikke en claude/-branch).

1. git checkout main && git pull --rebase origin main. Mangler GitHub-adgang, så stop og skriv til NAVN, hvad der mangler.
2. Læs README.md og CLAUDE.md og følg reglerne. Skriv kun i NAVNs egne filer (log/navn/, status/navn.md).
3. Læs ALT, hvad ANDEN har pushet siden sidste aften: git log --since="26 hours ago" --stat, og læs de ændrede filer – ANDENs logs, status/anden.md, nye filer i beslutninger/, ændringer i CLAUDE.md og eventuel kode.
4. Skriv et kort resumé i NAVNs log for i dag (log/navn/<ÅÅÅÅ-MM-DD>.md) under "## Nyt fra ANDEN": hvad ANDEN har lavet, nye beslutninger, og hvad det betyder for NAVNs arbejde. Findes loggen ikke, så opret den med linjen "Ingen log skrevet i dag." over resuméet. Opfind ikke arbejde.
5. Commit, git pull --rebase origin main, git push origin main.
6. Afslut med resuméet til NAVN (højst 5 punkter). Har ANDEN ikke pushet noget, så skriv det.
---
