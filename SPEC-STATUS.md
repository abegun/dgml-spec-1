# Spec Status

**Build on this spec — it's stable enough for production use today. We are not locking v1.0 until implementers outside the founding organizations have pushed on it.**

## What "stable" means right now

- The core architecture — docsets, namespaces, `dg:origin` grounding, `dg:itemprop`/`dg:href` semantic links, and the DGMLX package/attestation format (spec.md §§1–10) — is settled. We do not expect these to change shape.
- Specific attribute names, edge-case handling, and less-central sections (e.g., user-directed extraction schemas, §13) are still open to change based on real feedback.
- Any breaking change made before v1.0 will be called out explicitly, with a migration note — see the [Spec stability tracking issue](https://github.com/dgml-io/dgml-spec/issues/6) — not buried silently in a diff.

## Why it's not v1.0 yet

v1.0 means we stop making breaking changes without a major version bump. We're not ready to make that promise until the spec has been exercised by implementers outside Docugami and Inveniam. That's the point of this launch: we want your document types, your edge cases, and your objections before anything locks.

## Current version

The spec has iterated through internal drafts up to `0.7` (see the header in [`spec.md`](spec.md)). The first formally tagged public release will be `v0.1` — a deliberate reset marking the start of an explicit, public versioning policy, not a downgrade in maturity. See [ROADMAP.md](ROADMAP.md) for the path from there to `v1.0`.

## How to give feedback

- Found an error, ambiguity, or inconsistency in the spec? Open an [Issue](../../issues).
- Have a use case, a question, or want to propose a change? Open a [Discussion](../../discussions).
- See [CONTRIBUTING.md](CONTRIBUTING.md) for the full process, including the CLA.

## License

Apache 2.0. See [LICENSE](LICENSE).
