# MCP Wars Command: interface releases

Signed interface bundles for MCP Wars Command, the operator client for macOS, iPhone and iPad. This repository holds release assets only; it has no source.

Each release carries `manifest.json`, `manifest.sig` (Ed25519 over the manifest's exact bytes) and `bundle-<version>.tar.gz`. Installed apps download the latest release without a token, verify the signature against the public key compiled into them and the archive's SHA-256 and size, and run it on trial with automatic rollback. A file that does not verify is never used, so the hosting being public does not let anyone change what the apps run.
