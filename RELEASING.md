#  RELEASING.md
```markdown
## Releasing tHttp

This document defines the release process for the **tHttp** project.

## Versioning
We adhere to [Semantic Versioning (SemVer)](https://semver.org/).
- **Current Version:** 1.0.0

## Release Steps
1. **Update Metadata:** Ensure `Cargo.toml` reflects the new version.
2. **Update Changelog:** Add new features/fixes under a new version header.
3. **Verification:** Run `cargo test --workspace` to ensure stability.
4. **Git Tagging:**
   ```bash
   git tag -a v1.0.0 -m "Release version 1.0.0"
   git push origin main --tags
   ```
5. **Deployment:** Binary artifacts are generated and attached to the GitHub release.

