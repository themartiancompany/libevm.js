
[comment]: <> (SPDX-License-Identifier: AGPL-3.0)

[comment]: <> (----------------------------------------------------)
[comment]: <> (Copyright © 2024, 2025, 2026  Pellegrino Prevete)
[comment]: <> (All rights reserved)
[comment]: <> (----------------------------------------------------)

[comment]: <> (This program is free software: you can redistribute)
[comment]: <> (it and/or modify it under the terms of the GNU Affero)
[comment]: <> (General Public License as published by the Free)
[comment]: <> (Software Foundation, either version 3 of the License.)

[comment]: <> (This program is distributed in the hope that it will be)
[comment]: <> (useful, but WITHOUT ANY WARRANTY; without even the)
[comment]: <> (implied warranty of MERCHANTABILITY or FITNESS FOR A)
[comment]: <> (PARTICULAR PURPOSE.)

[comment]: <> (See the GNU Affero General Public License for more)
[comment]: <> (details. You should have received a copy of the GNU)
[comment]: <> (Affero License along with this program.)
[comment]: <> (If not, see <https://www.gnu.org/licenses/>.)
[comment]: <> (SPDX-License-Identifier: AGPL-3.0)

# EVM Library (`libevm.js`)

Library providing useful functions
to write native applications interacting with EVM-compatible
blockchain networks.

It depends on
[Crash Javascript](
  https://github.com/themartiancompany/crash-js),
[EVM Chains Info](
  https://github.com/themartiancompany/evm-chains-info),
[EVM Chains Explorers](
  https://github.com/themartiancompany/evm-chains-explorers),
the
[EVM Contracts Tools](
  https://github.com/themartiancompany/evm-contract-tools)
and it is supposed to be used with
[EVM Wallet](
  https://github.com/themartiancompany/evm-wallet)
and
[Solidity Compiler](
  https://github.com/themartiancompany/solidity-compiler).

The build reference tool for applications using the library
is
[EVM Make](
  https://github.com/themartiancompany/evm-make).
For this Javascript implementation is `npm`.

Together with the aforementioned applications
as well as others, libEVM makes up the EVM Toolchain.

EVM stands for *Ethereum Virtual Machine*.

Significant applications developed using the library are
the
[Ethereum Virtual Machine File System](
  https://github.com/themartiancompany/evmfs)
(EVMFS), the
[Ur](
  https://github.com/themartiancompany/ur)
uncensorable Life and DogeOS user repository
and application store and its reference
[pub](
  https://github.com/themartiancompany/pub)
publishing tool and source retrieval tool
[aspe](
  https://github.com/themartiancompany/aspe),
the
[EVM OpenPGP Key Server](
  https://github.com/themartiancompany/evm-openpgp-keyserver),
the uncensorable, undeletable, distributed, network-neutral,
decentralized Twitter (whose sources are entirely hosted on
the EVMFS) and many others currently in development.

LibEVM is a core component of the Human Instrumentality Project (HIP).

## Documentation

You can immediately start using this library into your Bash program by
pasting the following at its beginning:

```bash
_bin="$(
  dirname \
    "$( \
      command \
        -v \
	  "env")")"
_lib="${_bin}/../lib"
source \
  "${_lib}/libevm/libevm"
```

For a Javascript program or library you can use a similarly styled
import:

```javascript
const
  _libevm_module =
    require(
      "libevm");
```

While one could say documentation work is never really
complete for a program or library in active development,
a short manual can be consulted upon installation typing

```bash
man \
  libevm
```

It's currently suggested to look at existing programs
depending on the library to speed up the library usage
understanding.

## Installation

The library in this source repo
can be installed from source using GNU Make.

```bash
make
make \
  install
```

LibEVM has officially published on the
the uncensorable
[Ur](
  https://github.com/themartiancompany/ur)
user repository and application store as
`libevm`.
The source code is published on the
[Ethereum Virtual Machine File System](
  https://github.com/themartiancompany/evmfs)
so it can't possibly be taken down.

To install it from there just type

```bash
ur \
  libevm
```

A censorable HTTP Github mirror of the recipe published there,
containing a full list of the software dependencies needed to run the
tools is hosted on
[libevm-ur](
  https://github.com/themartiancompany/libevm-ur).

A censorable binary build for the GNU and Android bases of
Life and DogeOS, also compatible with the Arch Linux distribution
and the Termux pacman-based environment can be found on the
[Fur](
  https://github.com/themartiancompany/fur)
and it can be installed by typing

```bash
fur \
  libevm
```

Direct links to the binary package can be directly accessed
through
[Github](
https://github.com/themartiancompany/fur/tree/libevm)

The package has also been published
on the NPM Registry as
[`evm-chains-info`](
  https://npmjs.com/package/libevm)
and so it can be installed from there by typing

```bash
npm \
  install \
    "libevm"
```

## License

This program is released by Pellegrino Prevete under the terms
of the GNU Affero General Public License version 3.
