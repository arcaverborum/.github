# AI policy

Arca Verborum is **AI-assisted and human-owned**.

- AI tools are welcome for finding sources, extracting and transforming data,
  checking quality and drafting. The person who opens a pull request **owns
  every changed record**, as if they had typed it.
- **Disclose AI use** in the pull-request template's *AI assistance* field:
  `none`, `search & suggestion`, `extraction or transformation`, or
  `drafting & review`, plus the tool used. CI checks that the field is filled.
  Each release summarizes these fields.
- **Agents never approve or merge.** Automated agents may open issues or draft
  pull requests under a clearly named bot account; a human must take a pull
  request over before it can be merged.
- **A model's review is never expert review.** Do not describe model checks as
  independent, expert or gold-standard validation, in the data or in papers.
- The schema-A baseline was built by the maintainer with extensive AI
  assistance; releases and papers say so.
