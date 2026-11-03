# A first look at Arca Verborum

*For the colleagues invited to edit Arca Verborum and to co-author its data paper.*

Thank you for joining. This page explains what Arca Verborum is, what we ask
of you in this first round, and how to report what you find. Neither git nor
any programming is needed to take part.

## What Arca Verborum is

- **One curated record per language variety.** Lexibank and similar
  collections keep every source side by side. Arca Verborum instead chooses,
  for each variety, the best available lexical evidence, and builds one
  reviewed wordlist from it. Every form keeps its source, citation and
  licence.
- **Shared identifiers.** Varieties are mapped to Glottolog and concepts to
  Concepticon and WordNet, with source-specific cognate judgements kept as
  published.
- **Static and reproducible.** Every release is a set of files, and anyone
  can rebuild it byte for byte from the repository and the release's input
  snapshot. The first release is `A-2026-11-03`: about 2.1 million forms for
  7,371 varieties from 226 sources.
- **Built on Lexibank.** Lexibank's contribution is foundational; most of the
  data come through it, together with GLED, Wiktionary and original sources.
  The project began as a way for students to use comparative lexical data
  without learning a toolchain or cloning hundreds of repositories.

## What we ask in this first round

Look at the languages you know best and tell us what is wrong or could be
better. A few hours is plenty; you do not need to check everything.

1. **Open the explorer** at <https://arcaverborum.org>. Until the domain
   moves, use <https://arcaverborum.github.io/site/>.
2. **Find your varieties.** Search by name, Glottocode or ISO code, or browse
   by family. Each variety page shows its source, coverage, forms and
   cognate sets; a comparison table can put up to 16 varieties side by side.
3. **Check, in particular:**
   - **Source choice.** Is this the best source for the variety? Is there a
     better or more recent one we missed?
   - **Readings.** Each form shows how its segments were obtained: from the
     source's own IPA, through a documented orthographic profile,
     re-segmented, or unresolved. Is a spelling being treated as a
     pronunciation? Are tone, length or other contrasts lost?
   - **Meanings.** Is the form mapped to the right concept? Are senses too
     broad or too narrow?
   - **Identity.** Is the variety the one it claims to be (Glottocode, name,
     dialect or historical stage)?
   - **Cognacy** as given by the source, where you know it to be wrong.

## How to report

- **Easiest:** open an issue with the
  [Data problem](https://github.com/arcaverborum/arcaverborum/issues/new?template=data-problem.md)
  form. Give the variety identifier (`av_id`, shown on every variety page),
  the concept, what is wrong, and your evidence (source, page or URL).
- **For several changes, or if you use git:** open a pull request; the
  repository's `ONBOARDING.md` explains how. Every pull request states
  whether and how AI tools were used (see the
  [AI policy](AI_POLICY.md)), and CI rebuilds the affected varieties
  automatically.
- **A new source** can be contributed in a pull request as a small
  "source extension"; the repository's `extensions/README.md` describes the
  format.
- A short e-mail to Tiago is fine too.

## Your role as an editor

- Send Tiago your **GitHub login**, your **ORCID** and the **language
  families** (one or more) you would like to look after.
- You will then be listed in `editors.csv`, and GitHub will ask you to review
  every pull request that touches your families. Decisions about your
  languages are yours. If a request waits more than 30 days, the maintainer
  may merge it and give the reason in the pull request.
- You can merge any pull request whose checks pass, your own included.
- See [CONTRIBUTING](CONTRIBUTING.md) for the details.

## Authorship and next steps

- **Everyone invited is a co-author** of the data paper: your earlier
  discussions and your review of your own languages are the contribution.
  The order is Tiago first, then alphabetical.
- After this first look, the release is deposited on **Zenodo** with a DOI,
  and the editors are listed as contributors.
- The data paper (planned for MDPI *Data*) is drafted in a private
  repository, which you will be invited to.

## Downloads

Each release has three downloads, which differ only in the source licences
they include:

| Download | Contents |
|---|---|
| `full` | everything, including two sources whose terms are still being clarified |
| `redistributable` | sources whose licences allow redistribution |
| `by` | CC BY and public-domain sources only |

The input snapshot needed to rebuild the release is also attached. All of
them are on the
[releases page](https://github.com/arcaverborum/arcaverborum/releases/latest).
