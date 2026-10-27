# release-propagate-lab

End-to-end lab for the `propagate` workflow of
[getplumber/plumber](https://github.com/getplumber/plumber). **Not a real
release**: nothing here is published to users.

- `.github/workflows/propagate.yml` is a copy of the real workflow that
  targets the lab component
  [gitlab.com/getplumber/examples/component-release-lab](https://gitlab.com/getplumber/examples/component-release-lab)
  instead of `gitlab.com/getplumber/plumber`, and has no website job.
- `templates/plumber.yml` carries the real templates of v0.7.9 to v0.7.12
  (real image digests), with a few lab commits in between to exercise the
  GitLab release notes.
- Dispatch "Propagate Release" with the latest version on `main`.

Used for [getplumber/plumber#569](https://github.com/getplumber/plumber/issues/569).
