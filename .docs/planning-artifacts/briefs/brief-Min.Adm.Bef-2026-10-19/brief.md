---
title: "Product Brief: Min.Adm.Bef"
status: final
created: 2026-10-19
updated: 2026-10-19
---

# Product Brief: Min.Adm.Bef

## Executive Summary

In a Norwegian Armed Forces (Forsvaret) unit, the administrative officer (*adm bef*) manages the unit's materiel and issues it to personnel as needed. Today, unclassified stock such as consumables is tracked with pen and paper or in Excel sheets on a PC that is rarely at the storage site. Because nobody can trust the numbers, the admin staff physically count every warehouse every week.

Min.Adm.Bef is a mobile-friendly website. Each adm bef sets up their unit's warehouses and stock, and everyone in the unit registers what they take out or bring in, from their phone, at the shelf. Personnel can also send requests for materiel (*behovsinnmeldinger*) to the adm bef, who answers what can and cannot be met. Each unit is isolated behind its own unit code, so units see only their own warehouses.

The goal is simple: an always-current stock overview that is trustworthy enough to cut physical counts from weekly to monthly. The product is built as a school project, but it comes from the author's daily experience of this problem in the military.

## The Problem

- **No overview where the work happens.** Stock records live on paper or in Excel on a PC away from the warehouse. The adm bef cannot check stock levels while standing in the storage room or away from the office.
- **Transactions go unrecorded.** Items are taken out and delivered without a reliable trail of who did what and when.
- **Counting is the safety net, and it is expensive.** Because the records cannot be trusted, the admin staff (*adm søylen*) count physical stock weekly.
- **Requests are informal.** Needs reach the adm bef by word of mouth or messages, with no shared record of what was asked for and what was answered.
- **SAP is not the answer for this stock.** Forsvaret's existing system, SAP, handles sensitive materiel. It is not readily available on a phone and is not where everyday consumables get tracked.

## The Solution

A website that works well on a phone, with two roles:

- **Adm bef:** creates and manages warehouses and items, sees all stock and the full transaction history, answers requests, runs stock counts, sets low-stock thresholds, and hands the role over on rotation.
- **User (unit personnel):** registers every withdrawal and delivery, and sends requests to the adm bef.

Core capabilities in v1:

1. **Unit isolation by code.** Each unit gets a unit code. Users join their unit with it and see only that unit's warehouses. The code belongs to the unit, not the person, and survives rotations.
2. **Warehouses and stock.** The adm bef defines the unit's warehouses and the items held in each.
3. **In/out transactions.** Every withdrawal and delivery is registered by the person doing it. Stock changes *only* through these transactions.
4. **Requests (*behovsinnmelding*).** Users submit a need, and the adm bef replies whether it can be met. A request never changes stock by itself. Stock changes only when the materiel is actually issued and registered.
5. **Stock count (*telling*).** The adm bef enters physical counts. The app shows deviations from expected stock and records the correction.
6. **Low-stock warnings.** The adm bef sets a minimum level per item and is warned when stock drops below it.
7. **Handover.** The outgoing adm bef transfers the role to the incoming one, and all history is kept. The new adm bef decides whether to change the unit code.

## What Makes This Different

This is not a clever technical moat. It is a fit to the job:

- **At the shelf, not at the desk.** It is designed for the phone in the storage room, which paper and Excel cannot match.
- **Deliberately narrow.** It covers only unclassified (UGRADERT) stock. It does not compete with SAP; it covers the everyday consumables SAP is not used for.
- **Built by a user.** The workflow comes from someone who does this work, not from a requirements document.

## Who This Serves

- **Primary: the adm bef.** Responsible for the unit's materiel. Success means trusting the numbers without counting every week, and handing over a clean history to their successor.
- **Secondary: unit personnel.** They need to take and return materiel quickly and to ask for what they need. Success means logging takes seconds and requests get a clear answer.
- **Indirect: the unit commander (*sjef*).** Their directive that everything is logged is what makes the data trustworthy.

## Success Criteria

- **Primary:** physical counts drop from weekly to monthly, and the monthly count shows deviations within a tolerance each unit's adm bef sets.
- Every withdrawal and delivery in the unit is registered in the app.
- Registering a transaction on a phone takes under 30 seconds.
- Every request gets an answer from the adm bef.
- **School deliverable:** a working website, usable on a phone, that demonstrates the v1 capabilities with test data.

## Scope

**In v1:** everything listed under *The Solution*, as a mobile-friendly website with individual logins and two roles.

**Out of v1:**
- Classified or sensitive materiel. It stays in SAP.
- Integration with SAP.
- Personal equipment signed out to individuals.
- Ordering from suppliers.
- Offline mode, which is not needed.

## Security and Privacy Constraints

- **UGRADERT only.** No classified information may be entered.
- **Pseudonymous identity.** Users are shown by real name only if personnel security allows it. Otherwise each user is identified by role and an individual number. The adm bef keeps the key linking numbers to people in a BEGRENSET (restricted) document *outside* the app.
- **Aggregation is decided per unit.** A full overview of a unit's stock can reveal more than any single item does. Whether a unit may use the app is decided per unit. The school project uses test data only.

## Key Assumptions and Risks

- **Logging discipline comes from command, not code.** Accuracy depends on everyone logging every transaction, which depends on a clear directive from the commander. The app's job is to make logging so easy that following the directive costs almost nothing.
- **Approval for real use.** Using the app in a real unit requires that unit's approval, including where it is hosted and whether it may be used on phones. The school project does not resolve this.

## Vision

If it proves itself, Min.Adm.Bef becomes the standard pocket tool for unclassified stock across Forsvaret units. It would give every adm bef an overview they can trust, a clean handover on rotation, and hours back every week that now go to counting.
