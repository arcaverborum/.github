# Contributing to Arca Verborum

Arca Verborum is curated by editors. Anyone may propose a change; editors
merge it.

## How changes are made

- **Every change is a pull request** to `master`, including the maintainer's.
  A pull request may be merged once **CI passes**; no approving review is
  required.
- **CODEOWNERS** (generated from `editors.csv`) automatically asks the
  language editors of the affected varieties and families to review. When a
  variety has a language editor, wait for that editor before merging a change
  to its source choice or readings. Changes to shared code, the concept
  catalog or the schema go through the maintainer or a layer editor.
- If a language editor has not responded within **30 days**, the maintainer
  may merge, stating the reason in the pull request.
- Pipeline-wide, non-curatorial changes (re-normalization, schema migration)
  carry the `bulk/mechanical` label, applied only by the maintainer. They do
  not wait for language editors.
- Fill in the pull-request template, including the **AI assistance** field.

## Roles

| Role | Who | Scope |
| --- | --- | --- |
| Maintainer | Tiago Tresoldi | pipeline, schema, releases, policy |
| Editor | members of the `editors` team | may merge any pull request with green CI |
| Language editor | editors with a scope in `editors.csv` | varieties, families (one or more) or a layer (`concepts`, `colexification`, `pipeline`) |

`editors.csv` is data: it generates `.github/CODEOWNERS`, the contributors of
each release's Zenodo record, and the explorer's "editors of this variety".

## Working on a language

1. Clone the repository and download the accepted-inputs snapshot of the
   latest release; unpack it at the repository root (see `ONBOARDING.md`).
2. Edit `varieties/<av_id>/` (config, `custom/` files, recipe) and rebuild
   with `python build.py update <av_id>`.
3. Open a pull request. CI rebuilds every touched variety from the snapshot.
4. A new source or variety whose rows are not in the snapshot ships its
   reviewed intake rows as a snapshot extension in the same pull request.

## Evidence

Keep source transcriptions, derived profiles, semantic judgments and
source-specific cognacy explicit. A spelling is not IPA because it tokenizes.
Record tone, quantity, phonation, dialect or stage, exact senses and source
provenance. Put supporting evidence under `docs/evidence/` and cite it from
the variety's files.
