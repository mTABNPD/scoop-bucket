# scoop-bucket

mTAB's Scoop bucket. Hosts manifests for mTAB-internal CLIs distributed publicly as Windows x64 binaries.

## Install

```
scoop bucket add mtab https://github.com/mTABNPD/scoop-bucket
scoop install mtab/halo
scoop install mtab/pde
```

The `mtab` short bucket name is local to your scoop install — pick whatever you like; the URL is what matters.

## Update

```
scoop update halo
scoop update pde
```

## Available manifests

| Manifest | Description | Source |
|---|---|---|
| `halo` | CLI for the Halo platform | [mTABNPD/halo-platform-cli](https://github.com/mTABNPD/halo-platform-cli) |
| `pde` | Internal mTAB developer CLI | [mTABNPD/mtab-pde-cli](https://github.com/mTABNPD/mtab-pde-cli) |

## Platforms

Currently Windows 10 21H2+ / Server 2019+ x64 only. The binaries are not yet Authenticode-signed — running from a terminal works without prompts, but Explorer double-clicks may show a SmartScreen warning until signing is wired up.
