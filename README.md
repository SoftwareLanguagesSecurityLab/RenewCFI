# RenewCFI
Renew is a framework that provides support for Control-Flow Integrity to dynamically generated code.

Details about Renew can be found in the paper "Renewable Just-In-Time Control-Flow Integrity."

## Overview

Renew is implemented as several components, which are contained in separate git repositories.
These consist of *Miniverse*, the main rewriting component of Renew, *SupersetDisassembler*, the disassembly component, and *PageAlloc*, a simple memory allocator.

## Miniverse

The code for Miniverse can be found [here](https://github.com/SoftwareLanguagesSecurityLab/RenewCFI-Miniverse).  This requires the *SupersetDisassembler* and *PageAlloc* components to be installed in order to work.

## SupersetDisassembler

The superset disassembler code can be found [here](https://github.com/SoftwareLanguagesSecurityLab/RenewCFI-SupersetDisassembler).  This requires the *PageAlloc* component to be installed, and it also relies on the udis86 disassembler for linear disassembly.

Our fork of udis86 with some fixes for some instructions we encountered can be found [here](https://github.com/SoftwareLanguagesSecurityLab/udis86).  We highly recommend you use this version.

## PageAlloc

The code for PageAlloc can be found [here](https://github.com/SoftwareLanguagesSecurityLab/RenewCFI-PageAlloc).  It doesn't have any special dependencies.
