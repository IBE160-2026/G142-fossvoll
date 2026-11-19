# Markedsresearch Your Gym

## 2026-11-19 kl. 14:50 — jfossvoll

### Oppgave
Undersøke om treningsbrukere (særlig nybegynnere) vil betale for Your Gym. Hypotesen til Jens: folk bryr seg mer om kroppen enn før, og «progressive overload» gjør at sets og reps-logging betyr noe. I tillegg kom et konseptskifte, se under. Det ble også notert to brainstorming-ideer. Underveis i økten ble statuslinjen satt opp; det er en global innstilling og logges ikke her.

### Plan
- Kjørte `bmad-deep-recon` (Run, market + user-voice, standard preset). Tre parallelle researchere: betalingsvilje, etterspørsel og frafall, og konkurrenter med forretningsmodell. Deretter en egen andre runde med kontrollsøk.
- Rapport: `.docs/planning-artifacts/research/market-gym-independent-workout-app-willingness-2026-11-19/research.md`. Digests ligger i `digests/`, og prosessloggen i `.memlog.md`.

### Resultat
- Rapporten er ferdig: 26 kilder, 13 påstander i ledgeren (5 verifisert, 7 uverifisert, 1 omstridt). Den mekaniske sitatsjekken er ok.
- Hovedfunn:
  - Styrketrening vokser, særlig blant Gen Z.
  - Bare et mindretall logger i app.
  - Rundt 3–4 % av dem som laster ned en treningsapp, betaler.
  - Prisnivå i Norge: Hevy/Strong ca. 235–325 kr/år, Fitbod ca. 879–1 190 kr/år.
  - Ingen konkurrent viser én økt som et rom der avataren går mellom maskinene.
  - Gamification gir små effekter, og de avtar over tid.
- Konseptskifte bestemt av Jens: kartet er ikke lenger treningssenterets plantegning. Det er et rektangulært rom der maskinene står i øktens rekkefølge, med målstrek i enden, og avataren går fra maskin til maskin. Produktet blir uavhengig av treningssenter, med B2C framfor white-label.
- Brainstorming-ideer fra Jens:
  1. Med det nye konseptet blir loggingen raskere og smidigere.
  2. Brukerreisen: logg inn → lag avatar → sett mål → lag økter med eller uten KI → start på første maskin → logg økten → velg om den skal publiseres (som Strava/Hevy).
- Hoppet over for å holde kjøringen rask: semantisk sitatsjekk med egen subagent, HTML-briefing og doc-standards-pass via bmad-review.
- Research-filene er ikke committet. Bare loggfilene committes av denne skillen.

### Åpne punkter
- Oppdater product brief for Your Gym med konseptskiftet (rom i øktrekkefølge, uavhengig av senter, B2C/freemium) og brukerreisen.
- Test betalingsvilje hos 5–10 nybegynnere med en prototype. Ingen studie av dette ble funnet.
- Les Reddit (r/fitness, r/beginnerfitness) manuelt. Verktøyene ble blokkert.
- Hent norske tall: medlemstall i Virkes fullrapport og SATS Healthier & Happier 2025.
