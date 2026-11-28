# SR-MPLSv6

Working draft of **IPv4 Traffic over an IPv6-Only Segment Routing MPLS
Underlay Network** (`draft-swer-spring-sr-mplsv6`).

The draft proposes network layer awareness for forwarding IPv4 traffic
over IPv6-only SR-MPLS infrastructure without an additional service label.
It covers penultimate hop popping, Explicit NULL label selection, ultimate
hop popping, and IPv6 Traffic Engineering Router ID requirements.

This is a work in progress. Unresolved questions are recorded in
Appendix A, “Open Issues”.

## Read the draft

- [HTML editor’s copy](https://daryll-swer.github.io/SR-MPLSv6/)
- [Plain text](draft-swer-spring-sr-mplsv6.txt)
- [XML source](draft-swer-spring-sr-mplsv6.xml)

The HTML copy is published from the parent repository’s `main` branch.
For proposed changes, download the `internet-draft` artifact from the
pull request’s successful build run.

## Edit and build

Edit the XML source, using one sentence per line.
Building requires Python 3 with
[xml2rfc](https://pypi.org/project/xml2rfc/), `make`, and Node.js with `npx`.

```sh
make          # Generate HTML and text in build/; refresh the repository TXT
make idnits   # Check the draft
```

Commit the XML and regenerated TXT together.
Do not edit the generated TXT directly.

## Contribute

Open an issue or pull request to suggest changes.
Read [CONTRIBUTING.md](CONTRIBUTING.md) for editing guidance and the
applicable IETF contribution policies.
