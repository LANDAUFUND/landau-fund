# Antigravity Direction Development Protocol

Status: active from 2026-05-25.

This protocol governs how Landau Fund develops the `Антигравитация` direction across GitHub, the public website/domain layer, Bitrix24, reviewer coordination, and release governance.

It complements, but does not replace:

— `docs/ANTIGRAVITY_PUBLICATION_PROTOCOL.md`;
— `docs/PUBLIC_PRIVATE_BOUNDARY.md`;
— `REPOSITORIES.md`;
— the release-candidate, review, machine-evidence, human-review, and outreach packages in `LANDAUFUND/antigravity-open-research`.

## 1. Controlling Principle

The direction must develop as an auditable open-research program, not as a set of disconnected documents.

Every meaningful action must answer five questions:

1. What is being developed?
2. Where is the source of truth?
3. Is it public, private, protected, or secret?
4. What review gate applies before publication or public promotion?
5. Where is the action recorded?

If any answer is unknown, the default status is `HOLD / ТРЕБУЕТ ПРОВЕРКИ`.

## 2. Non-Negotiable Rules

Antigravity is not to be described as proven unless a future release explicitly passes the required scientific, data, license, patent, security/privacy, and human-review gates.

The default release decision remains `NO-GO` until written review conclusions and nonconformity closure records exist.

Public repositories contain only public-safe, approved, citable material.

Private repositories contain drafts, raw work, internal review, patent-sensitive materials, and operational coordination. Private material is not public licensed automatically.

Secrets never belong in GitHub, Bitrix24 documents, website files, memory files, logs, or final answers. Use 1Password references and approved wrappers.

The confirmed project domain is `landau.website`. Production DNS, redirects, hosting, or CMS changes require an explicit source-of-truth decision before execution.

The confirmed Bitrix24 live anchor is `LANDAU.FUND | Лев Давидович Ландау`, group ID `620`. Do not use old cached `LANDAU FOUNDATION` anchors without separate live verification.

## 3. System Map

### Institutional Public Root

Repository:
https://github.com/LANDAUFUND/landau-fund

Role:

— institutional registry;
— repository map;
— authorship and license policy;
— public/private boundary;
— direction development protocol;
— website/stub source artifacts until production source is confirmed.

This repository is the correct place for governance documents that explain how the overall direction is run.

### Public Research Repository

Repository:
https://github.com/LANDAUFUND/antigravity-open-research

Role:

— public research packages;
— released methodologies;
— public templates;
— public release-candidate and review packages;
— citable documentation;
— public changelog and publication record.

This repository is the correct place for materials that are meant to be public, reusable, and citeable.

### Private Laboratory Repository

Repository:
https://github.com/LANDAUFUND/antigravity-lab-private

Role:

— internal drafts;
— raw notes and measurements;
— patent-sensitive material;
— private review preparation;
— internal coordination;
— materials before public release review.

This repository is the correct place for work that should not yet be part of the public record.

### Website And Domain Layer

Canonical domain:
https://landau.website

Role:

— public front door;
— short status statement;
— links to GitHub repositories;
— contact path;
— license and attribution notice;
— scientific disclaimer.

Until the production source is confirmed, website artifacts in `website/` are staging artifacts only. They do not prove that the live site has been deployed.

### Bitrix24 Operational Archive

Confirmed anchor:
`LANDAU.FUND | Лев Давидович Ландау`, group ID `620`.

Role:

— operational archive;
— Disk copy of important packages;
— file IDs and folder IDs;
— hash verification records;
— live feed status posts;
— internal continuity record for Codex and project operators.

## 4. Visibility Classes

Every new file, issue, website item, email, or Bitrix24 artifact must be classified before work starts.

### Public

Allowed in public GitHub and on the website.

Examples:

— approved methodology;
— public-safe review protocol;
— public changelog;
— public issue or discussion;
— public landing page copy;
— CC BY 4.0 document notice.

### Private

Allowed only in the private lab repository or confirmed internal Bitrix24 area.

Examples:

— drafts;
— raw lab notes;
— internal review comments;
— unapproved hypotheses;
— reviewer coordination before public disclosure;
— operational planning.

### Protected

Allowed only after explicit placement decision and access control.

Examples:

— patent-sensitive details;
— exact promising experimental parameters;
— partner-sensitive materials;
— private reviewer identities before approval;
— access-control records.

### Secret

Not allowed in GitHub or documents.

Examples:

— passwords;
— API keys;
— tokens;
— private keys;
— recovery phrases;
— cookies;
— full environment values.

Secret values must stay in 1Password or another approved secret manager.

## 5. Standard Work Unit

Each meaningful development step should be treated as a work unit.

A work unit must have:

— short title;
— date;
— owner or responsible role;
— target repository or system;
— visibility class;
— source materials;
— output files;
— review gates;
— publication record;
— changelog entry;
— memory update when operationally important.

Large work units should be packaged as a directory with:

— `README` or protocol file;
— CSV registry when tracking decisions, people, files, or evidence;
— SHA-256 sums when file integrity matters;
— clear status: `DRAFT`, `REVIEW`, `RELEASE CANDIDATE`, `NO-GO`, `HOLD`, or `RELEASED`.

## 6. GitHub Development Workflow

For governance or infrastructure changes:

1. Work in `LANDAUFUND/landau-fund`.
2. Update the relevant protocol or registry.
3. Update `README.md`, `REPOSITORIES.md`, or `CHANGELOG.md` when the change affects public navigation.
4. Commit with a clear message.
5. Push to GitHub when the content is public-safe.

For public research releases:

1. Start from the private lab repository unless the material is already public-safe governance.
2. Prepare a public-safe package.
3. Check secrets, privacy, partner sensitivity, authorship, license, patent risk, and scientific wording.
4. Copy only approved material into `antigravity-open-research`.
5. Update public README/index/changelog.
6. Commit and push.
7. Create or update a public issue/discussion for important release records.

For private development:

1. Keep drafts and raw work in `antigravity-lab-private`.
2. Do not grant public license by default.
3. Do not copy protected material into public GitHub.
4. Move toward public release only through the publication and review gates.

## 7. Website And Domain Protocol

The website layer must be conservative.

Minimum public landing/stub content:

— `Landau Fund`;
— `Antigravity Open Research Initiative`;
— current status as open research, not proven technology;
— links to `LANDAUFUND/landau-fund` and `LANDAUFUND/antigravity-open-research`;
— link to license and citation policy;
— contact path using a confirmed mailbox;
— scientific disclaimer;
— no private repository links unless intentionally disclosed;
— no donation/payment claims before legal and financial review.

Production deployment requires a separate decision:

1. Confirm the website source of truth.
2. Confirm hosting or CMS access.
3. Confirm DNS or redirect target.
4. Confirm HTTPS status.
5. Deploy only public-safe content.
6. Verify the live page in a browser.
7. Record the deployment in GitHub, Bitrix24, and project memory.

Until that decision exists, `website/` files in GitHub are templates or staging artifacts, not proof of live deployment.

## 8. Review And Release Gates

The default release status is `NO-GO`.

A final public release can move to `GO` only when all required gates are closed:

— scientific review;
— data review;
— license review;
— patent review;
— security/privacy review;
— human reviewer conclusions;
— nonconformity closure;
— hash and archive verification;
— final release-board decision.

Machine checks improve traceability but do not replace human review.

Outreach logs do not prove reviewer participation.

Templates do not prove execution.

Draft release notes do not create a final release.

## 9. Public Communication Rules

Use precise wording:

— `research direction`;
— `open research initiative`;
— `experimental framework`;
— `hypothesis under review`;
— `not established as proven`.

Avoid unsupported wording:

— `proven antigravity`;
— `working antigravity technology`;
— `confirmed breakthrough`;
— `final release`;
— `peer reviewed`, unless the review is actually complete and documented.

Public communication should point to GitHub evidence instead of broad claims.

## 10. Operating Cadence

For each new layer:

1. Define the work unit and visibility class.
2. Place it in the correct repository.
3. Add review and publication records.
4. Push public-safe GitHub changes.
5. Mirror important operational packages to Bitrix24 when appropriate.
6. Update local memory after substantial work.

Recommended public cadence:

— small governance updates: immediate when public-safe;
— research packages: only after review gate preparation;
— site updates: only after source and deployment path are confirmed;
— final releases: only after GO decision.

## 11. Immediate Direction Plan

### Phase A: Protocol Lock

Create and publish this protocol.

Make it visible from the root repository and public research repository.

Keep the private repository aligned with the same public/private boundary.

### Phase B: Website Source Decision

Choose the production source for `landau.website`:

— GitHub Pages/static site;
— existing hosting;
— CMS;
— temporary redirect/stub.

No DNS or production changes before this decision.

### Phase C: Public Stub

Prepare a minimal public website/stub that links to GitHub and states the scientific status conservatively.

### Phase D: Review Execution

Move from templates and logs to real reviewer assignment, NDA/COI where needed, written conclusions, and NC closure.

### Phase E: Release Decision

Only after Phase D can a release board record `GO`, `GO WITH LIMITATIONS`, `NO-GO`, or `DEFER`.

## 12. Memory Rule

After substantial work:

— update local project memory;
— update the global memory index only if a new memory file is created;
— update the canonical Landau Fund memory file when the state changes;
— mirror important memory to the confirmed Bitrix24 anchor when appropriate;
— never store real secrets.
