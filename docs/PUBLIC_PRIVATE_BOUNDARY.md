# Public and Private Boundary

Status: active from 2026-05-24.

The Antigravity direction uses separate public and private repositories.

## Public Means Public

Public repositories are intended to be visible, citable, linkable, indexed, and reused.

Public repositories may contain:

— released research texts;
— approved public laboratory reports;
— methodologies;
— diagrams;
— tables;
— public templates;
— citation metadata;
— authorship records;
— changelogs;
— public issues and discussions.

Public repositories must not contain:

— secrets;
— passwords;
— API keys;
— private keys;
— private contact data;
— raw internal coordination;
— partner-sensitive materials;
— unapproved drafts;
— claims that have not been marked as preliminary or reviewed.

## Private Means Private

Private repositories are internal workspaces.

Private repositories may contain:

— drafts;
— lab planning;
— raw notes;
— raw measurements;
— internal review;
— operational coordination;
— unpublished hypotheses;
— release checklists.

Private repositories must still avoid storing real secrets in files. Secrets belong in 1Password or another approved secret manager, not in Git history.

## Release Gate

A private file becomes public only after explicit release action:

1. Check for secrets and private data.
2. Check scientific status and wording.
3. Add attribution and source links.
4. Add the correct license.
5. Move or copy to the public repository.
6. Commit with a clear message.
7. Update changelog.
8. Create a public issue or discussion if public proof of publication is needed.
