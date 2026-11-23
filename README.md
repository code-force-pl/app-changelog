# Code Force — App Changelog

Public release history of the **Code Force** courses app
([main repo](https://github.com/MatZajc/course_platform_2_0)).

Every entry in [`CHANGELOG.md`](./CHANGELOG.md) is one deployment: a dated,
versioned summary of everything that landed on `master` since the previous
release. The app itself does not embed this changelog — this repository is the
single, shareable record of what shipped and when.

## Versioning

Versions are date-based: `vYYYY.MM.DD` (e.g. `v2026.11.23`). If more than one
release happens on the same day, they get a `-2`, `-3`, … suffix.

## How a release is written

1. Every merge to `master` in the main repo adds a pending entry file under
   `docs/changelog/` (enforced by a pre-push hook).
2. At deploy time the pending entries are summarised into one release section
   and appended to `CHANGELOG.md` here.
3. The pending files are then pruned from the main repo — history lives only
   in this repository.

See the `changelog` skill and `docs/changelog/README.md` in the main repo for
the full workflow.
