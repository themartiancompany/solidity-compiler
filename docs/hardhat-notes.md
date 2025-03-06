# Centralized blockchain explorers verification

For centralized blockchain explorers which require for
contract verification to build a contract with the
Hardhat backend, as they require
providing the solidity source code file together with
a so-called `metadata.json` file (solc might be able to
generate that file as well but I haven't been able to
check still), be aware the `metadata.json` file they
want is the one in the `build-info` output directory.
