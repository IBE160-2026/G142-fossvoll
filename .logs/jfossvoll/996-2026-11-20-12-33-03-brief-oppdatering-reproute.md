# Brief-oppdatering RepRoute

## 2026-11-20 kl. 12:33 — jfossvoll

### Oppgave
Oppdatere product brief for Your Gym med konseptskiftet fra markedsresearchen (se [997-markedsresearch-your-gym](997-2026-11-19-14-50-07-markedsresearch-your-gym.md)). Jens ville gå gjennom endringene med coaching. Til slutt skulle briefen ferdigstilles, økten logges, og alt committes og pushes.

### Plan
- Kjørte `bmad-product-brief` i Update-modus med coaching-path. Briefen ble revidert i samme mappe, og de gamle white-label-beslutningene ligger som historikk i briefens `.memlog.md`.
- Avklarte motstrid med tidligere beslutninger: kunde, maskiner, prismodell, publisering og hva som skulle fjernes. Deretter navn, målgruppe, avatar-mekanikk, prototype-omfang og animasjoner.
- Gjorde et kort websøk på lisenser for gratis øvelsesbiblioteker (wger, free-exercise-db, GIF-datasett).

### Resultat
- Briefen `.docs/planning-artifacts/briefs/brief-Your Gym-2026-10-18/brief.md` heter nå **RepRoute** (arbeidsnavn) og har status final. Commit 21e09c3.
- Beslutninger:
  - Kun B2C freemium. Gratis logging. Én Premium-pakke med KI-bygde økter og kosmetikk.
  - Salg til treningssentre (fellesskap) er en mulig senere utvidelse.
  - Primær målgruppe er nybegynnere. Sekundær er folk som aldri har brukt en treningslogg. Erfarne Hevy-brukere er ikke målgruppe.
  - Maskiner: brukeren velger maskin per øvelse, og de plasseres i øktens rekkefølge. Valgfri utstyrsliste lar KI-en lage økter med maskinene brukeren har.
  - Avataren er koselig, rund og elskelig. Den blir sterkere etter en økt, men går alltid tilbake til normal form. Den blir bare lei seg når brukerens eget ukemål ikke nås. Inspirert av Duolingo-uglen.
  - KI-en foreslår et realistisk ukemål ut fra treningserfaring. XP og nivåer er gratis.
  - Prototypen har 5–10 øvelser med animasjon. Anbefalingen er 2D-animasjoner laget i Claude Code der avataren selv utfører øvelsen, med wger og free-exercise-db som faglig referanse.
  - Publisering av økter, ekte Premium-betaling og native apper er utenfor prototypen. Plattformen er en responsiv webapp med mobil først.
- Fjernet fra briefen: gym-branding, ansattvisning av maskinbruk, kartbygging per senter og pilot-mål.
- `addendum.md` har fått seksjonen «Pivot to RepRoute» med regler for avatar, mål og maskiner til PRD-en.
- Markedsresearchen fra forrige økt er også committet (21e09c3).
- Statuslinjen ble endret tidligere i økten. Det er en global innstilling i `~/.claude/`, utenfor repoet.
- Doc-standards-passet ble gjort inline, ikke via `bmad-review`-subagenter.

### Åpne punkter
- Kjør `bmad-prd` basert på RepRoute-briefen (står allerede i issues.md).
- Sjekk om navnet RepRoute er ledig i App Store, Google Play og som varemerke.
- Velg 5–10 øvelser og avklar kilde for korrekt teknikk før animasjonene lages.
