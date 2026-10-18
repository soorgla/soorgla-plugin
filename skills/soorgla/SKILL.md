---
name: soorgla
description: >-
  Research Turkish law with the Soorgla MCP server: find Turkish court decisions
  (Yargıtay, Danıştay, Anayasa Mahkemesi, Sayıştay, KİK, regional and first-instance
  courts), read current statute articles and their amendment history, search the
  Official Gazette (Resmî Gazete), and answer with links to the original texts on
  soorgla.com. Use whenever "Soorgla", "soorgla.com", a soorgla.com/karar or
  soorgla.com/mevzuat link, or the user's request to use Soorgla comes up.
---

# Soorgla

Soorgla is a read-only research index of Turkish primary legal sources: court
decisions and legislation. The `soorgla` MCP server bundled with this plugin acts as
the signed-in Soorgla user. None of its tools change data.

## Working with the results

1. **Cite what the tools return.** Every result carries a ready citation
   (`kaynak.markdown` or `markdown_citation`) that links to the source page on
   soorgla.com. Put it next to the claim it supports. Do not build soorgla.com URLs
   yourself and do not cite a decision or article the tools did not return.
2. **Statute numbers are not unique.** The same number can belong to a law and a
   regulation. When a lookup returns several candidates, pick by title and type, or
   ask the user.
3. **Free text works.** Case search is semantic: describe the facts in a sentence
   (Turkish works best) instead of listing keywords.
4. **Dates matter.** Statute text and deadlines change over time. Say which version
   or date the answer relies on when it is not the current text.

## Scope and limits

- Information only, not legal advice. Say so when the user asks about their own
  situation, and suggest consulting a lawyer for a specific case.
- Content is in Turkish. Answer in the user's language, but quote legal text as
  returned.
- A Soorgla account is required. The first connection opens Soorgla sign-in in the
  browser (OAuth).
