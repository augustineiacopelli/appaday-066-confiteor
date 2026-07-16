# Confiteor

**App 066 of the [AppADay](https://augustineiacopelli.github.io/appaday/) project** · Category: Spirituality · Shipped 2026-07-12

A private, offline companion for the Sacrament of Reconciliation, named for the *Confiteor* — the "I confess" prayer. It walks you through the whole arc of the sacrament rather than serving as one more examination checklist, and it is built for the nervous and the long-absent as much as for the regular penitent.

**Live:** https://augustineiacopelli.github.io/appaday-066-confiteor/

## What it does

- **Examination of conscience.** A full examination through the Ten Commandments, mirroring the same 129-sin reference list used by Daily Examen (App 054) so the two stay in step. Tap any sin to flag it; an inline panel lets you record how many times it was committed and attach a private note, all in one place. Every sin carries an info button with a plain-language explanation of what it means, to help tell the vaguer ones apart.
- **Venial or mortal, discerned properly.** Sins that are objectively grave matter are tagged, and a further set are tagged "can be grave" — matter that rises to grave only when it is serious. Flagging either opens a short discernment: was there full knowledge, and deliberate consent (and, for the circumstantial kind, was the matter serious). Both conditions met reads as possibly mortal; either missing reads as venial. A plain-language guide explains the three conditions.
- **A private list you carry in.** The Review screen gathers everything you flagged, with a live counter of mortal, venial, and still-to-weigh, per-sin notes, and multiplicity counts.
- **The rite, step by step.** Read the steps anytime, or enter a large-type "in the confessional" mode you can hold while kneeling. Your greeting line is pre-filled with the time since your last confession, and your list appears at the confessing step with **mortal sins ordered first**, each with its count and note.
- **Prayers.** Prayer before confession, three forms of the Act of Contrition (traditional, contemporary, and the short "Lord Jesus, have mercy on me, a sinner"), the Confiteor, a thanksgiving, and Psalm 51.
- **Confession log.** A running record of your confession dates, kept in its own storage separate from your flagged list so it survives everything routine. The most recent date drives the home screen and the greeting.

## Privacy and data safety

Everything stays on the device. There is no account, no server, and no AI reading your conscience.

- Your flagged list and confession log are stored locally, each mirrored to a backup key, with corrupt-read protection so damaged data is set aside rather than silently discarded.
- The app requests persistent storage so compliant browsers will not evict your data; Settings reports the protection status honestly.
- **Encrypted backups.** Export a password-protected file (AES-256-GCM via the Web Crypto API, key derived with PBKDF2) that only you can open, and import it back — merging, never overwriting. Your password is the only key and cannot be recovered.
- An optional "forget on close" mode wipes the flagged list each session while keeping your log.

## Built with

Vanilla HTML, CSS, and JavaScript in a single file. No frameworks, no build step, no external dependencies beyond Google Fonts (Cormorant Garamond, EB Garamond, Inter). Encryption uses the browser's built-in Web Crypto API. Designed mobile-first with a candlelit-confessional aesthetic and a confessional-screen lattice motif.

## Note

This is a devotional aid, not an authority. Its gravity tags and discernment prompts follow standard Catholic moral teaching but are meant to help you think, not to render a verdict. When you are unsure, name it in confession and let the priest help you weigh it.
