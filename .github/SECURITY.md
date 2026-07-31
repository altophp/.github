# Security policy

Alto treats security reports as private until a fix and disclosure are ready.
Please do not open a public issue for a suspected vulnerability.

This is the default security policy for the `altophp` organization. It applies
to any repository under this org that does not carry its own `SECURITY.md`.

## Supported versions

Before a package's `1.0.0`, development snapshots receive best-effort fixes on
`main`, with no stable maintenance promise.

After `1.0.0`, each package supports the latest stable minor release of its
current major line. Users on an earlier minor or major release must update to
that version unless an advisory explicitly names another supported branch.

| Release line | Security support |
| --- | --- |
| Unreleased `main` before 1.0 | Best effort |
| Latest stable minor of the current major | Supported |
| Earlier minor or major | Update required unless an advisory says otherwise |

## Report a vulnerability

If GitHub displays a **Report a vulnerability** button for the affected
repository, use it to open a private report. Otherwise, email
[smn.andre@gmail.com](mailto:smn.andre@gmail.com) with the subject
`[SECURITY] alto/<package>`, naming the affected package.

Include:

- the affected package and version or commit;
- relevant configuration (options, policies, extensions) involved;
- a minimal non-destructive reproduction;
- the security impact and required attacker capabilities;
- any known workaround or suggested fix;
- whether the report may be shared with other maintainers.

Do not include secrets, personal data, or production credentials. Use local or
synthetic data in proofs of concept.

A package's own documentation, where it exists, defines its specific security
boundaries (for example a curated-HTML policy or a resource confinement
guarantee). Report an issue when a package violates a boundary it documents.
Expected, documented behavior is not a vulnerability by itself.

## Response and disclosure

These are response targets, not a service-level agreement:

1. Acknowledge the report within three business days.
2. Provide an initial assessment within ten business days.
3. Send a status update at least every fourteen days while work continues.
4. Coordinate a fix, release, advisory, and reporter credit before public
   disclosure.

The default coordinated-disclosure target is 90 days after acknowledgement.
The maintainer and reporter may agree to a different date. Active exploitation
or a broadly available public proof may require an earlier advisory.

For a published package, the advisory will identify affected and fixed
versions. A GitHub Security Advisory and CVE will be requested when
appropriate so Composer and Packagist users can receive ecosystem alerts.
