# did-moify

did-modify is a command line go utility that detects modified git files. Below you can find the the availability and usage.

### Installation

You can install the did-modify utility for a specific OS at https://github.com/chef/file-mod/releases

Currently available for:
OS | ARCH
--- | ---
Darwin | x86-64 (amd64)
Linux | x86-64 (amd64)
Windows | x86-64 (amd64)

### Build

You can optionally build did-modify via the [goreleaser](https://goreleaser.com/) utility. Goreleaser uses a `.goreleaser.yml` to define how you would like to build and release your go binary(ies).

### `did-modify`

<!-- stdout "./build/linux/did-modify --help" -->
```
Prints "true" to STDOUT if any files matching GLOBS were modified between HEAD and GITREF. Otherwise, prints "false".

Usage:
  did-modify [flags]

Flags:
      --git-ref string   A valid Git reference (e.g. HEAD, master, origin/master, etc). (default "HEAD~1")
      --globs strings    Comma-separated list of glob patterns to inspect to determine if there are changes. (default [*])
  -h, --help             help for did-modify
```
<!-- stdout -->
