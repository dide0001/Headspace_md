# Headspace_md

Fælles repo for Diego og Aviajas afsluttende eksamensprojekt (multimediedesign) for headspace Danmark.
Repoet er både vores **fælles hukommelse for Claude** og hjemsted for **WordPress-temaet**.

## Sådan undgår vi konflikter

Reglen er enkel: **man skriver kun i sine egne filer.**

| Mappe / fil | Hvem må skrive | Indhold |
|---|---|---|
| log/diego/ | kun Diego (og Diegos Claude) | én fil pr. dag: ÅÅÅÅ-MM-DD.md |
| log/aviaja/ | kun Aviaja (og Aviajas Claude) | én fil pr. dag: ÅÅÅÅ-MM-DD.md |
| status/diego.md | kun Diego | hvad jeg arbejder på, og hvad der mangler |
| status/aviaja.md | kun Aviaja | samme for Aviaja |
| beslutninger/ | begge – men kun **nye filer** | én fil pr. beslutning: ÅÅÅÅ-MM-DD-emne.md. Gamle filer rettes ikke – en ændret beslutning bliver en ny fil |
| CLAUDE.md | kun når vi begge er enige | faste fakta og regler for Claude |
| wordpress-tema/ | den der koder (Diego) | temaets kode |

Fordi to personer aldrig skriver i den samme fil, kan Git altid flette automatisk.

## Rutinen

1. **Før man starter:** git pull --rebase – og bed Claude læse CLAUDE.md, begge status-filer, de nyeste filer i beslutninger/ og alt, hvad den anden har pushet siden sidst (git log + den andens logs). Claude skal kende den andens arbejde, før den går i gang.
2. **Når man stopper:** bed Claude skrive dagens log og opdatere sin statusfil, og derefter git add -A && git commit && git pull --rebase && git push.
3. **Hver aften** kører en planlagt opgave hos hver af os (oprettet på claude.ai/code/routines med repoet valgt). Den puller, læser alt, hvad den anden har pushet siden sidste aften, skriver et kort resumé i sin egen log under "Nyt fra …", pusher og sender en besked. Se opgaver/aften-sync.md.
