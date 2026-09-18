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
├── icons/         # Repository/package icons
├── Packages       # APT package index
├── Packages.gz    # Compressed APT package index
├── Release        # APT repository metadata
└── index.html     # Repository website
```

## Website

The repository website automatically reads `Packages` and displays the published package catalog, including:

- package name
- version
- architecture
- description
- package size

When new packages are published, the catalog updates automatically after the repository workflow finishes.

## Publishing packages

Only packages for which redistribution is permitted should be published.

After a permitted `.deb` is added to `pool/`, GitHub Actions:

1. rebuilds `Packages` and `Packages.gz`;
2. regenerates `Release` checksums;
3. deploys the repository website and APT metadata to GitHub Pages.

## Status

Repository infrastructure and automatic deployment are ready.
