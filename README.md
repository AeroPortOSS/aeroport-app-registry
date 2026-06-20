# aeroport-app-registry

This repository hosts the centralized application catalog data feed that powers the storefront window inside the native `aeroport-core` macOS application.

## Manifest Layout

All app tracking indices are defined within `manifest.json`. Every application listing provides exact download sources, cryptographic file verification hashes, required runtime environment parameters, and silent installation arguments (e.g., quiet, headless switches) used to configure target applications smoothly without popping full guest interactive windows.

## Code Contribution Guidelines

We accept community contributions to scale the volume of verified applications available in the ecosystem. To register a new verified Windows application:
1. Fork this repository.
2. Modify `manifest.json` following the structural property rules defined inside `schema.json`. Ensure all silent installation arguments are fully tested inside an unactivated Windows 11 ARM64 environment.
3. Submit a public Pull Request back to this repository.

Submissions will undergo a verification procedure by the maintainer team to confirm structural formatting accuracy, clean software packaging, and to optimize the initial initialization scripts.

## License

The structured definitions and configuration data within this tracking database are explicitly dedicated to the public domain under the Creative Commons CC0 1.0 Universal License.
