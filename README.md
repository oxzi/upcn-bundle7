# µPCN's Python Bundle7 Implementation

This repository contains a modified Python implementation of the [Bundle
Protocol Version 7 version 12][dtn-bpbis-12] based on the [Micro Planetary
Communication Network (µPCN) version 0.6.0][upcn] created by [Ingenieurbüro
Marius Feldmann (IMF)][marius-feldmann]. The original code was based on the
[10th version of the Bundle Protocol Version 7][dtn-bpbis-10].


## Changes

### Version 10 → Version 11

- CRC32 uses CRC32C (Castagnoli) instead of a PKZIP CRC-32
- CRC representation is in network byte order (*already implemented that way*)
- The *"block data length"*-field was removed from the Canonical Bundle Block
- Bundle Age is represented in microseconds instead of seconds (*no code was
  changed*)

### Version 11 → Version 12

No relevant changes were made.


[dtn-bpbis-10]: https://tools.ietf.org/html/draft-ietf-dtn-bpbis-10
[dtn-bpbis-12]: https://tools.ietf.org/html/draft-ietf-dtn-bpbis-12
[upcn]: https://upcn.eu/
[marius-feldmann]: http://www.marius-feldmann.de/
