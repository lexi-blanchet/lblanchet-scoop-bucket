# Scoop Bucket Template

[![Tests](https://github.com/lblanchet/lblanchet-scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/lblanchet/lblanchet-scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/lblanchet/lblanchet-scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/lblanchet/lblanchet-scoop-bucket/actions/workflows/excavator.yml)

Template bucket for [Scoop](https://scoop.sh), the Windows command-line installer.

## How do I use this template?

1. Generate your own copy of this repository with the "Use this template"
   button.
2. Allow all GitHub Actions:
   - Navigate to `Settings` - `Actions` - `General` - `Actions permissions`.
   - Select `Allow all actions and reusable workflows`.
   - Then `Save`.
3. Workflow permissions:
   - Navigate to `Settings` - `Actions` - `General` - `Workflow permissions`.
   - Ensure `Read repository contents and packages permissions` is selected.
   - Then `Save`.
4. Document the bucket in `README.md`.
5. Replace the placeholder repository string in `bin/auto-pr.ps1`.
6. Create new manifests by copying `bucket/app-name.json.template` to
   `bucket/<app-name>.json`.
7. Commit and push changes.
8. If you'd like your bucket to be indexed on `https://scoop.sh`, add the
   topic `scoop-bucket` to your repository.

## How do I install these manifests?

After manifests have been committed and pushed, run the following:

```pwsh
scoop bucket add lblanchet-scoop-bucket https://github.com/lblanchet/lblanchet-scoop-bucket
scoop install lblanchet-scoop-bucket/jellium-desktop-nightly
```
