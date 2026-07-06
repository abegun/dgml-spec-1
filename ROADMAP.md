# Roadmap

This roadmap covers the **DGML format specification** — schema, semantics, and versioning. It does not cover the reference implementation; that roadmap lives in [dgml-io/dgml](https://github.com/dgml-io/dgml).

It reflects our priorities for the next 3–6 months following the public launch. See [SPEC-STATUS.md](SPEC-STATUS.md) for the one-paragraph version of where things stand right now.

## Guiding principle

The spec is stable enough to build on today. It is not frozen. Between now and v1.0, we'd rather take a breaking change that fixes a real problem an implementer hit than lock in a mistake for the sake of stability theater. Every theme below exists to make that trade-off legible instead of ad hoc.

## Themes

### 1. Spec stability

Keep the core structural primitives — docsets, namespaces, `dg:origin`, `dg:itemprop`/`dg:href`, the `dg:` reserved attribute set, and the DGMLX package/attestation model — from changing shape without a documented, versioned migration path.

- [ ] Mark which `spec.md` sections are "core" (unlikely to change shape) vs. "still evolving" (open to change based on feedback)
- [ ] Document a deprecation/migration policy for any breaking change made before v1.0 locks

Tracked in [#6](https://github.com/dgml-io/dgml-spec/issues/6).

### 2. Community feedback process

Right now feedback has no defined home or response expectation. This theme is about making "open an issue" actually work: where things go (Issues vs. Discussions), who triages, and how a proposal moves from "raised" to "decided."

- [ ] Publish issue/PR triage expectations (response-time target, who's on point)
- [ ] Stand up the steering committee referenced in [CONTRIBUTING.md](CONTRIBUTING.md)
- [ ] Add issue templates for "spec bug," "spec change proposal," and "new sample contribution"

Tracked in [#7](https://github.com/dgml-io/dgml-spec/issues/7).

### 3. Format versioning

Define what a version number means for this spec, and what has to be true before we call something `v1.0` and stop making breaking changes without a major bump.

- [ ] Adopt a versioning policy for the spec itself — independent of DGMLX's per-document/per-anchor versioning (already specified in spec.md §10), which is unrelated
- [ ] Decide the public release numbering scheme going forward (the spec is currently at `0.7` internally; no public releases have been tagged yet)
- [ ] Define the criteria for locking `v1.0` — e.g., a minimum number of independent implementations, real-world document types validated beyond the founding organizations, and a quiet period with no open breaking-change proposals

Tracked in [#8](https://github.com/dgml-io/dgml-spec/issues/8).

## Out of scope for this window

- Formal submission to a standards body (OASIS, ISO, etc.) — premature before v1.0 locks.
- Multi-language reference implementations — that's implementation work, tracked in the [`dgml`](https://github.com/dgml-io/dgml) repo, not here.

## How to influence this roadmap

Open an [Issue](../../issues) or [Discussion](../../discussions). If your use case doesn't fit one of the three themes above, that's useful signal too — say so.
