# Convenient Mariner Containers

Unofficial and unsupported containers that I find useful for my work on [CBL-Mariner](https://github.com/microsoft/CBL-Mariner).

I'm only supporting 2.0 containers, since I don't do much work on 1.0 anymore. I build both amd64/aarch64 containers, because I am an Apple Silicon Enjoyer.

## Versioning

The versioning schema is semver-shaped. The major version matches that of the base Mariner container, the minor version is bumped every time the base container image version is updated, and the patch version is bumped when updating the container without a base image version update.

All images will be released for every tag update.

## Other curiosities

Images are signed using [cosign] using [fulcio] keyless signatures and [rekor] transparency logs. Use `COSIGN_EXPERIMENTAL=1 cosign verify <image>` to verify that signature.

[cosign]: https://github.com/sigstore/cosign
[fulcio]: https://github.com/sigstore/fulcio
[rekor]: https://github.com/sigstore/rekor
