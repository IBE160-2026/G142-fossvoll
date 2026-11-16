# Prosjektoppsett og git-kobling

## 2026-11-16 kl. 16:22 — jfossvoll

### Oppgave
Lage `CLAUDE.md` og `README.md` for Your Gym, deretter erstatte dem med versjonene fra GitHub-repoet `IBE160-2026/G142-fossvoll`, og koble den lokale prosjektmappen til repoet slik at `git pull` fungerer.

### Plan
- Skrev først egne `CLAUDE.md`/`README.md` basert på product brief i `.docs/planning-artifacts/briefs/brief-Your Gym-2026-10-18/`.
- Klonet repoet til en midlertidig mappe og kopierte inn `CLAUDE.md` og `README.md` fra GitHub (overskrev de egenproduserte).
- `git init`, la til `origin`, `git fetch`, `git reset origin/main` (beholdt arbeidskopien), satte `main` til å tracke `origin/main`.
- Hentet kun filer som manglet lokalt fra `origin/main`.

### Resultat
- `CLAUDE.md` og `README.md` er identiske med GitHub-versjonene (gruppe G142, sesjonslogg-regel).
- Mappen er et git-repo på `main` som tracker `origin/main` (siste commit f0113e0). Ingen lokale filer avvek fra GitHub.
- Hentet inn fra GitHub: `.gitignore`, `tilbakemelding-product-brief.md`, `.docs/planning-artifacts/architecture/technology.md`, briefen for Min.Adm.Bef og `.claude/skills/sesjonslogg/`.
- `gh` er ikke innlogget; push krever `gh auth login`.

### Åpne punkter
Ingen.
