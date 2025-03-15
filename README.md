[comment]: <> (SPDX-License-Identifier: AGPL-3.0)

[comment]: <> (-------------------------------------------------------------)
[comment]: <> (Copyright © 2024, 2025  Pellegrino Prevete)
[comment]: <> (All rights reserved)
[comment]: <> (-------------------------------------------------------------)

[comment]: <> (This program is free software: you can redistribute)
[comment]: <> (it and/or modify it under the terms of the GNU Affero)
[comment]: <> (General Public License as published by the Free)
[comment]: <> (Software Foundation, either version 3 of the License.)

[comment]: <> (This program is distributed in the hope that it will be useful,)
[comment]: <> (but WITHOUT ANY WARRANTY; without even the implied warranty of)
[comment]: <> (MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the)
[comment]: <> (GNU Affero General Public License for more details.)

[comment]: <> (You should have received a copy of the GNU Affero General Public)
[comment]: <> (License along with this program.)
[comment]: <> (If not, see <https://www.gnu.org/licenses/>.)

# Solidity compiler

Bash written
[Solidity](
  https://github.com/ethereum/solidity)
compiler using
[Hardhat](
  https://github.com/NomicFoundation/hardhat)
and solc as backends.

```bash
solidity-compiler \
  <contract>
```

It depends on the
[Crash Bash](
  https://github.com/themartiancompany/crash-bash)
library and uses
[GNU Indent](
  https://www.gnu.org/software/indent)
to properly parse Hardhat configuration
files at runtime to create run-once projects.

It is a dependency for
[EVM Make](
  https://github.com/themartiancompany/evm-make)
and so a build dependency for projects written
using the 
[libEVM](
  https://github.com/themartiancompany/libevm)
library.

This project is part of the EVM Toolchain.

## Usage

Help can be displayed by typing

```bash
solidity-compiler \
  -h
```

further informations are made available in
the manual.

```bash
man \
  solidity-compiler
```

Extra documentation is in the `docs` directory.

## Installation

The compiler in this source repo
can be installed from source using GNU Make.

```bash
make \
  install
```

The compiler has officially published on the
the uncensorable
[Ur](
  https://github.com/themartiancompany/ur)
user repository and Life and DogeOS
application store as `solidity-compiler`.
The source code is published on the
[Ethereum Virtual Machine File System](
  https://github.com/themartiancompany/evmfs)
so it can't possibly be taken down.

To install it from there just type

```bash
ur \
  solidity-compiler
```

A censorable HTTP Github mirror of the recipe published there,
containing a full list of the software dependencies needed to run the
tools is hosted on
[solidity-compiler-ur](
  https://github.com/themartiancompany/solidity-compiler-ur).

Be aware the mirror could go offline any time as Github and more
in general all HTTP resources are inherently unstable and censorable.

## License

This program is released by Pellegrino Prevete under the terms
of the GNU Affero General Public License version 3.
