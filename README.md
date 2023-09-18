# Convenient Azure Linux Containers

Unofficial and unsupported containers that I find useful for my work on [Azure Linux/CBL-Mariner] 2.0.

I build both amd64/aarch64 containers, because I am an Apple Silicon Enjoyer.

All containers come with `ca-certificates` pre-installed.

## Versioning

The versioning schema is semver-shaped. The major version matches that of the base Mariner container, the minor version is bumped every time the base container image version is updated, and the patch version is bumped when updating the container without a base image version update.

All images will be released for every tag update.

## Other curiosities

Images are signed using [cosign] with standard [fulcio] keyless signatures and [rekor] transparency logs. Use `cosign verify <image>` to verify that signature.

[Azure Linux/CBL-Mariner]: https://github.com/microsoft/CBL-Mariner
[cosign]: https://github.com/sigstore/cosign
[fulcio]: https://github.com/sigstore/fulcio
[rekor]: https://github.com/sigstore/rekor
