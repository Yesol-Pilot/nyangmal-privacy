# Repository Governance Contract

Policy ID: `ng-repo-governance/1.0.0`
Last reviewed: 2026-08-27

## Identity

- Repository: `Yesol-Pilot/nyangmal-privacy`
- Lifecycle class: `public-privacy-surface`
- Current owner: `Yesol-Pilot`
- Intended owner: `NeoGenesisAI`
- Canonical branch: `master`
- Canonical-branch target: `main`
- Visibility: `public`
- Production status: `UNKNOWN`
- Transfer state: `REQUIRED`

`UNKNOWN` means not independently verified and must never be reported as PASS.

## Purpose and current risk

This repository publishes privacy information for the Nyangmal product. Policy accuracy must be proven against the exact app, SDKs, network behavior, store declarations, and user controls.

- Active public URL, covered package and versions, data categories, processors, retention, deletion, and contact operation remain `UNKNOWN`.
- A static privacy page cannot be treated as proof that the runtime follows it.
- Analytics, advertising, purchases, sharing, device identifiers, crash reporting, storage, and external links require explicit reconciliation.
- Private user data, credentials, account exports, and incident evidence are prohibited in Git history.

## Required remediation

- [ ] Record package or app IDs, versions, operator, SDKs, processors, data categories, purposes, retention, transfers, rights, contact, and deletion path.
- [ ] Reconcile policy with source manifests, network behavior, analytics, ads, purchases, backend, store forms, and in-app disclosure.
- [ ] Run full-history secret, link, public-claim, personal-data, and legal-text drift audits.
- [ ] Add product-coverage, SDK inventory, URL, locale, store consistency, consent, deletion, accessibility, publication, and rollback checks.
- [ ] Normalize `master` to `main` only after public links and store references are verified.
- [ ] Transfer the repository to `NeoGenesisAI` while preserving redirects and store links.

## Pull-request and branch rules

- PRs declare affected product versions, data and SDK changes, processors, retention, rights, URL, and effective date.
- Review conversations resolve before squash merge.
- Canonical branches are not force-pushed or deleted.

## Exit criteria

The repository becomes `TRANSFERRED_COMPLIANT` only when organization ownership, exact runtime-to-policy reconciliation, user rights and deletion, public availability, store consistency, version history, and rollback are proven.

The presence of this file alone is not compliance.
