# March 2018 Hardfork Specification

Version Draft 0.1, 2017-01-29

## Summary
 
When the median time past[1] of the most recent 11 blocks (MTP-11) is greater than or equal to UNIX timestamp 1526400000 Bitcoin Cash will execute a hardfork according to this specification. Starting from the next block these consensus rules changes will take effect:

* Blocksize increase to 32 MB
* Re-enabling of several opcodes
* Canonical transaction ordering

The following are not consensus changes, but are recommendated changes for Bitcoin Cash implementations:

* Automatic replay protection for future hardforks
* Increase OP_RETURN relay size to 223 total bytes

## Blocksize increase

The blocksize hard capacity limit will be increased to 32MB (32000000 bytes).

## Opcodes

Several opcodes will be re-enabled per [may-2018-opcodes](may-2018-opcodes.md)