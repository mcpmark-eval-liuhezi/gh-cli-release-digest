# GitHub CLI v2.63.0 Release Digest

- **Display name:** GitHub CLI 2.63.0
- **Tag:** v2.63.0
- **Published:** 2024-11-27 (2024-11-27T21:10:54Z UTC)
- **Release page:** https://github.com/cli/cli/releases/tag/v2.63.0

## Summary of Changes (Highlights)

The v2.63.0 release of the GitHub CLI focuses on repository creation, attestation workflows, and documentation/UX polish:

- **Bare repository creation:** `gh repo create` now supports creating bare (empty) repositories.
- **Attestation improvements:** The `getAttestations` functions were refactored and verification results printing was updated, improving artifact attestation handling.
- **`gh pr view` enhancement:** An option was added to return the `baseRefOid` for pull requests.
- **Security documentation:** A section on manual verification of releases was added to the documentation.
- **Error handling:** `gh release create` now prints a friendly error when it fails due to a missing `workflow` OAuth scope.
- **Docs fixes:** Some multiline command documentation was fixed to use `heredoc` strings.

## Security Note

This release includes a security advisory (GHSA-jwcm-9g39-pmcw): a vulnerability was identified that could leak authentication tokens when cloning repositories containing git submodules hosted outside of GitHub.com and ghe.com. Details: https://github.com/cli/cli/security/advisories/GHSA-jwcm-9g39-pmcw

## New Contributors

@daliusd made their first contribution in this release.

**Full Changelog:** https://github.com/cli/cli/compare/v2.62.0...v2.63.0
