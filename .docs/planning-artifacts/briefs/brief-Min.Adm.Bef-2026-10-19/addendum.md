# Addendum: Min.Adm.Bef

Detail the user gave during discovery that belongs in downstream documents (PRD, architecture, UX) rather than the brief.

## Identity and access (for PRD / architecture)

- Each user has an individual login and joins a unit with the unit code.
- Two roles, adm bef and user. Permissions follow the role.
- Display identity is either a real name or role + individual number, depending on personnel security. The app must support the number-only mode. The mapping from number to person is never stored in the app.
- On handover, the adm bef role moves from the outgoing to the incoming person. Rotating the unit code is optional and up to the new adm bef. If it is rotated, existing members' access needs a defined behavior (open question for the PRD).

## Stock rules (for PRD)

- Stock changes only through registered in/out transactions and stock-count corrections.
- Requests (behovsinnmeldinger) are a communication channel only and never move stock.
- The stock count compares physical counts with expected stock, shows the deviation, and records the correction as its own logged event.

## Usage context (for UX)

- Primary device: a phone, used in the storage room.
- Connectivity is assumed at storage sites; no offline mode.
- Today's baseline: weekly physical counts by the admin staff, with pen and paper or Excel on a PC away from the site.
