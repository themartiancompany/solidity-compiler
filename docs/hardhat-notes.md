[comment]: <> (SPDX-License-Identifier: AGPL-3.0)

[comment]: <> (-------------------------------------------------------------)
[comment]: <> (Copyright © 2024, 2025, 2026  Pellegrino Prevete)
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

# Centralized blockchain explorers verification

For centralized blockchain explorers which require for
contract verification to build a contract with the
Hardhat backend, as they require
providing the solidity source code file together with
a so-called `metadata.json` file (solc might be able to
generate that file as well but I haven't been able to
check still), be aware the `metadata.json` file they
want is the one in the `build-info` output directory.

Centralized blockchain explorers contract verification
can be avoided though by deploying contracts using
[EVM Deployer](
  https://github.com/themartiancompany/evm-deployer),
which has support for uploading the source contract
code directly to the
[EVM Contracts Source Index](
  https://github.com/themartiancompany/evm-contracts-source-index).

The EVM Contracts Source Index hosts contracts
sources on-chain on the
[EVMFS](
  https://github.com/themartiancompany/evmfs)
and it is natively supported by the
[EVM Contracts Tools](
  https://github.com/themartiancompany/evm-contracts-tools),
which download the sources, build them locally
and perform the contract call, so greatly
streamlining the process of interacting
with a smart contract from inside a classical
computer program.
