# Contributing

This repository relates to activities in the Internet Engineering Task Force
([IETF](https://www.ietf.org/)). All material in this repository is considered
Contributions to the IETF Standards Process, as defined in the intellectual
property policies of the IETF currently designated as
[BCP 78](https://www.rfc-editor.org/info/bcp78),
[BCP 79](https://www.rfc-editor.org/info/bcp79), and the
[IETF Trust Legal Provisions (TLP) Relating to IETF Documents](https://trustee.ietf.org/license-info).

Any edit, commit, pull request, issue, comment, or other change made to this
repository constitutes a Contribution to the IETF Standards Process. You agree
to comply with all applicable IETF policies and procedures, including BCP 78,
BCP 79, the TLP, and the TLP rules regarding code components (e.g., being
subject to a Simplified BSD License) in Contributions. See the
[IETF Note Well](https://www.ietf.org/about/note-well/) for details.

## Editing the draft

- The source of truth is
  [`draft-swer-spring-sr-mplsv6.xml`](draft-swer-spring-sr-mplsv6.xml), written
  in RFC XML v3 ([RFC 7991](https://www.rfc-editor.org/info/rfc7991)).
- Authoring convention: one sentence per line, so that diffs stay reviewable.
- Keep artwork within 69 columns so that it fits the 72-column text output.
- For draft changes, run `make` and `make idnits`, then commit the XML and
  regenerated TXT together. After committing, run `make check-readable` to
  verify that the committed TXT matches the XML.
- The plain-text copy,
  [`draft-swer-spring-sr-mplsv6.txt`](draft-swer-spring-sr-mplsv6.txt), is
  generated from the XML. Do not edit it by hand. README-only and other
  documentation changes do not need regeneration; CI checks every pull request.
- Leave the draft revision unchanged for ordinary edits. Update `docName` and
  `<seriesInfo>` together when preparing an agreed IETF Datatracker submission.
- `make submit` generates expanded XML locally; it does not upload or submit
  the draft.
