# Tilbakemelding på product brief

| | |
|---|---|
| **Gruppe** | G142 – G142-fossvoll |
| **Product brief** | Ingen product brief funnet på main per 2026-10-06 (siste commit e63b03d) |
| **Tilbakemelding fra** | Faglærer i IBE160 (utarbeidet med KI-støtte) |
| **Dato** | 2026-10-06 |

## Samlet vurdering

- **Bør revideres før dere går videre.** Det ble ikke funnet noen product brief eller tilsvarende prosjektbeskrivelse på main per 2026-10-06. Lag en product brief før dere går videre til PRD og arkitektur.

**Hva vi fant i repoet:**

Repoet inneholder bare README.md (med medlemsliste) og .gitignore fra opprettelsen, og commit-historikken har bare den første commiten. Det finnes derfor ikke grunnlag for en foreløpig vurdering av vanskelighetsgrad og gjennomførbarhet.

Har dere en brief liggende lokalt, på en annen branch eller i et annet verktøy, må den committes og pushes til main i dette repoet. Sensor vurderer bare det som ligger i repoet.

## Hvorfor product brief er viktig for mappen

Product brief er utgangspunktet for PRD, arkitektur, stories og til slutt koden. Del 1 av mappen (applikasjon og prosess, 70 %) vurderes blant annet på om sensor kan følge en sporbar vei fra plan til ferdig app. Kriteriet «Prosess og KI-styring» teller alene 30 % av del 1, og sensor ser etter BMAD-dokumenter som faktisk er brukt og oppdatert over tid. Den vurderes også på om appen gjør det dere har beskrevet, om den er testet, om den er godt designet, og om den kan kjøres etter README.

Uten en brief mangler både dere og sensor et felles utgangspunkt for hva appen skal gjøre. Jo senere briefen kommer, jo vanskeligere blir det å vise en jevn og sporbar prosess, og jo mindre tid blir det til PRD, arkitektur, stories, implementering og testing.

## Hva briefen bør inneholde

Bruk BMAD-flyten: product brief → PRD → arkitektur → epics og stories → implementering med Claude Code. Skillen `bmad-product-brief` i BMAD hjelper dere å lage briefen gjennom en samtale. Faglærers eksempelprosjekt viser hvordan det kan se ut: https://github.com/IBE160-2026/beergame.

Briefen bør ha disse delene:

| Del av brief | Hva den bør svare på |
|---|---|
| Executive Summary | Hva er appen, og hvilket problem løser den? To–tre korte avsnitt. |
| The Problem | Hvem har problemet, i hvilke situasjoner, og hva gjør de i dag? Gi gjerne et konkret eksempel. |
| The Solution | Hva gjør brukeren i appen, steg for steg? Beskriv opplevelsen, ikke teknologien. |
| What Makes This Different | Hvilke alternativer finnes i dag, og hvorfor er deres løsning bedre for brukeren? Vær ærlig. |
| Who This Serves | Hvem er primærbrukeren? Beskriv én konkret bruker, ikke «alle». |
| Success Criteria | Hvordan vet dere at appen virker? Skriv kriterier som kan testes, f.eks. «brukeren kan registrere X og se det i oversikten». |
| Scope | Hva er med i første versjon («In»), og hva er bevisst utelatt («Out»)? |
| Vision | Hvor kan appen gå videre etter emnet, uten at det blåser opp første versjon? |

I tillegg bør briefen, eller en kort tilleggsfil, inneholde en **begrunnet vurdering av vanskelighetsgrad og gjennomførbarhet**:

- Sammenlign med forslagslista for emnet: enkel (f.eks. 1) AI Study Buddy eller 6) To-do-liste med smarte etiketter), middels (2) AI CV- og søknadsassistent, 7) Kurs-FAQ-chatbot) eller vanskelig (3) simulering av prosjektledelse, 4) MRP II, 5) KI-styrt sensurering).
- Vurder om første versjon realistisk kan bli ferdig og testet i løpet av semesteret, med tid til hele BMAD-flyten.
- Tenk gjennom om dere selv kan kontrollere at appen gir riktige svar, og om sensor kan kjøre appen etter README uten deres API-nøkler eller betalte kontoer (f.eks. med testmodus eller eksempeldata).

Et enkelt prosjekt gir stor sjanse for å bli ferdig, men krever mer i design, testing og dokumentasjon for å nå helt opp. Et vanskelig prosjekt gir større mulighet for toppkarakter, men også større risiko. Velg et nivå dere tror dere kan gjennomføre godt.

## Neste steg for gruppen

1. Bli enige om prosjektidé, gjerne med utgangspunkt i forslagslista eller en egen idé med en tydelig bruker og et konkret problem.
2. Lag en product brief med delene over, for eksempel med `bmad-product-brief`, og legg den i repoet (f.eks. under `_bmad-output/planning-artifacts/briefs/` eller `docs/`).
3. Ta med en kort, begrunnet vurdering av vanskelighetsgrad og gjennomførbarhet.
4. Commit og push briefen til main så snart som mulig, og gå deretter videre til PRD.

Oppdater product brief i repoet når dere gjør endringer, slik at historikken viser hvordan planen utviklet seg. Det er en del av prosessen sensor ser etter.
