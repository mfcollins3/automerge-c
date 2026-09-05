# Automerge-C

## Table of Contents

1. [About Automerge](#about-automerge)
1. [About this Repository](#about-this-repository)

## About Automerge

[Automerge](https://automerge.org/) is a "library of data structures for
building collaborative applications." Automerge is an implementation of
[conflict-free replicated data types](https://crdt.tech/), or **CRDT**s. CRDTs
allow collaboration on the same documents by multiple users on different
machines and enforces eventual consistency. CRDTs are able to resolve conflicts
between changes made by different users.

## About this Repository

This repository is used to build release packages of the
[Automerge-C](https://github.com/automerge/automerge/tree/main/rust/automerge-c)
library. Automerge-C provides a C API over the Automerge Rust library that can
be used to create Automerge mappings for different languages. The Automerge team
does not produce binary builds of the Automerge-C library when they tag new
releases. I created this repository to automate producing builds of the 
Automerge-C libraries for Apple macOS, Linux, and Microsoft Windows using GitHub
Actions so that I can use the libraries in my own applications or make it easy 
for others to use them in theirs.

I intend to keep this repository up-to-date with the latest releases by the
Automerge team. As they release new versions, I will update this repository and
rebuild the library packages to be consumed by other developers.

This repository produces builds of Automerge for the following platforms and
hardware architectures:

* Apple macOS
  * ARM64 (Apple Silicon)
* Linux
  * glibc, Intel x64/AMD64
  * glibc, ARM64
  * musl, Intel x64/AMD64
  * musl, ARM64
* Microsoft Windows
  * Intel x64/AMD64
  * ARM64

You can download the latest releases from the 
[Releases](https://github.com/mfcollins3/automerge-c/releases) page.

## License

For licensing terms on using the Automerge libraries, see the
[Automerge license](https://github.com/automerge/automerge/blob/main/LICENSE).

The source code in this repository (excluding the source code in the Automerge
Git submodule) is licensed under the [license](LICENSE.md).
