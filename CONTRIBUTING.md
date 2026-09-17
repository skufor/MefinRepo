# Adding packages

MefinRepo is intended to host packages that we are legally allowed to redistribute.

## Before adding a `.deb`

1. Make sure you created the package yourself, or have explicit permission to redistribute it.
2. Check the package license and any redistribution conditions.
3. Do not upload modified copies of third-party packages unless their license permits redistribution and modification.
4. Put permitted Debian packages under `pool/`.
5. After a push to `main`, GitHub Actions rebuilds `Packages`, `Packages.gz`, and `Release` automatically.

## Third-party packages

For packages that cannot be redistributed, document the original project/repository instead of copying the `.deb` into this repository.

## Security

Do not commit passwords, API keys, signing keys, certificates, or other secrets.
