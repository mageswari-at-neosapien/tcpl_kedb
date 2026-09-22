# Known error database

Root cause analyses are maintained as Markdown files with YAML front matter so people and agents can find and update them in this repository.

## RCA index

See [RCA_INDEX.md](RCA_INDEX.md) for ticket IDs, incident dates, issues faced, actions taken, and links to the detailed RCA files.

## File conventions

- Keep one RCA per file under `rcas/`, named `<ticket-id>-<short-description>.md`.
- Put YAML front matter between `---` delimiters at the start of each file.
- Use the metadata fields in the existing RCA as the initial schema: document identity and control, ticket, product, incident dates, ownership, tags, and source filenames.
- Quote identifiers, dates, times, and version strings. Use `YYYY-MM-DD` dates and `HH:MM` times. Use `null` for unknown metadata, and do not infer a timezone.
- Preserve the source document's creation and review dates. Record Markdown conversion and update dates separately in `markdown_created_date` and `markdown_updated_date`.
- Keep the front matter and body consistent when updating a record. Preserve reported-versus-confirmed distinctions, unknown values, action owners, and individual action statuses.
- Keep `RCA_INDEX.md` synchronized whenever a detailed RCA is added, updated, renamed, or removed. Commit related index and RCA changes together and use Git history to track revisions.
- Follow [AGENTS.md](AGENTS.md) for the required agent workflow and index checks.

## Source provenance

Ticket 636229 was converted from the supplied `RCA - Ticket 636229.docx`. The supplied PDF was identified by the requester as an equivalent copy. Source filenames are retained in front matter; the original attachments are not stored in this repository.

The RCA records findings and action statuses from the supplied document. Conversion to Markdown does not independently verify the incident or its resolution.
