# Scoop Bucket Template

## How do I install these manifests?

After manifests have been committed and pushed, run the following:

```pwsh
scoop bucket add lblanchet-scoop-bucket https://github.com/lblanchet/lblanchet-scoop-bucket
scoop install lblanchet-scoop-bucket/jellium-desktop-nightly
```

## Manifests

> [!WARNING]
> Nightly current has a [consistent issue](https://github.com/andrewrabert/jellium-desktop/issues/694) so i've guessed the last stable release

- [Jellium-desktop-stable](https://github.com/andrewrabert/jellium-desktop/actions/runs/31352217495)
- [Jellium-desktop-nightly](https://github.com/andrewrabert/jellium-desktop)
