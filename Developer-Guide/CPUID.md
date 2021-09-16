## Notes on CPU compatibility

List of required features. Note: `wide support` means *both* AMD and Intel.

Greentea OS targets CPUs **at least** from Q3 2011 and newer

- `SSE2` is mandatory on AMD64
- `NX` bit should be present on all AMD64, but may be disabled, does not affect system working
- `SSE3` wide support since 2005
- `CMPXCHG16B` wide support since 2006
- `PrefetchW` wide support since 2006
- `LAHF/SAHF` wide support since 2005
- `POPCNT` wide support since 2008
- `2 MB` huge pages seems to be mandatory on AMD64
- `I/O APIC` mandatory on multicore AMD64
- `ACPI 2.0` required by Tofita
- `SSE4.1` wide support since 2011 (CPU with SSE4.1 will have SSE3 and SSSE3)
- `SSSE3` wide support since 2011
- `SSE4.2` wide support since 2011

Optional features:

- `1 GB` huge pages (aka `PDPE1GB`) wide support since 2012 and used as optimization
- `x2APIC` is optional on AMD and **used** by Greentea if present
- `AVX` wide support since 2011 (except *all* Atoms, some modern Pentiums & Celerons, old Xeons)

Not required features:

- `SSE4a` seems like AMD-only and **not** used by Greentea
- `AVX2` introduced in 2013 and **not** used by Greentea (available for third-party apps)
- `AVX-512` introduced in 2016 and **not** used by Greentea
