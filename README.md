# MefinRepo

A lightweight APT repository for Sileo.

## Repository

**Source URL**

`https://skufor.github.io/MefinRepo/`

The repository metadata is generated automatically by GitHub Actions.

## Structure

```
MefinRepo/
├── pool/          # Published .deb packages
├── icons/         # Package/repository icons
├── Packages       # APT package index
├── Packages.gz    # Compressed APT package index
├── Release        # APT repository metadata
└── index.html     # Repository website
```

## Publishing packages

Third-party `.deb` files are not copied into this repository automatically.

Before a package is published, its original source and redistribution terms must be checked. Only packages that may legally be redistributed should be added to `pool/`.

After a package is added, GitHub Actions regenerates the APT indexes and deploys the updated repository.

## Status

The repository infrastructure is ready. Packages will be added after their redistribution permissions have been verified.
