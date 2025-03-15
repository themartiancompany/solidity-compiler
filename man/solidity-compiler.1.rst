..
   SPDX-License-Identifier: AGPL-3.0-or-later

   ----------------------------------------------------------------------
   Copyright © 2024, 2025  Pellegrino Prevete

   All rights reserved
   ----------------------------------------------------------------------

   This program is free software: you can redistribute it and/or modify
   it under the terms of the GNU Affero General Public License as published by
   the Free Software Foundation, either version 3 of the License, or
   (at your option) any later version.

   This program is distributed in the hope that it will be useful,
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU Affero General Public License for more details.

   You should have received a copy of the GNU Affero General Public License
   along with this program.  If not, see <https://www.gnu.org/licenses/>.


==================
solidity-compiler
==================

-----------------------------------------------------------
Solidity compiler
-----------------------------------------------------------
:Version: solidity-compiler |version|
:Manual section: 1

Synopsis
========

solidity-compiler *[options]* *contract_file*

Description
===========

Easy to use, easy to write bash Solidity Compiler
using Hardhat and solc under the hood.

It depends on the Crash Bash library and uses
GNU Indent to properly parse Hardhat configuration
files at runtime to create run-once projects.

It is a dependency for EVM Make and so a build
dependency for projects written using the LibEVM
library.

This project is part of the EVM Toolchain.

Options
=======

-b backend         Compiler backend.
-C solc_version    Version of the solc compiler to use.
-e evm_version     Ethereum virtual machine version.
-o out_dir         Output directory.
-w work_dir        Work directory
-d                 Whether to install developer dependencies.
-l                 Whether to delete the work directory
                   after a successful build.

-h                 Display help.
-c                 Enable color output.
-v                 Enable verbose output.

Bugs
====

https://github.com/themartiancompany/solidity-compiler/-/issues

Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.

See also
========

* evm-make
* evm-deployer
* libevm
* solc

.. include:: variables.rst
