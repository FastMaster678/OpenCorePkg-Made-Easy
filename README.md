<img src="/Docs/Logos/OpenCore_Made_Easy.png" width="400" height="155"/>

Welcome to OpenCore Made Easy! (DEFINITELY NOT OFFICIAL. To stay up to date with the latest builds of the real thing, see the [original repo](https://github.com/acidanthera/OpenCorePkg)).
-----

OpenCore bootloader, with generators to get OpenCore up and running fast without troubleshooting pain.

❗I haven't done anything yet! Come back when this fork is ready!❗


🕒In the meantime, you can check my Hello-World repository, which is under active development.

## Libraries

This repository also contains additional UEFI support common libraries shared by other projects in [Acidanthera](https://github.com/acidanthera). The primary purpose of the library set is to provide supplemental functionality for Apple-specific UEFI drivers. Key features:

- Apple disk image loading support
- Apple keyboard input aggregation
- Apple PE image signature verification
- Apple UEFI secure boot supplemental code
- Audio management with screen reading support
- Basic ACPI and SMBIOS manipulation
- CPU information gathering with timer support
- Cryptographic primitives (SHA-256, RSA, etc.)
- Decompression primitives (zlib, lzss, lzvn, etc.)
- Helper code for ACPI reads and modifications
- Higher level abstractions for files, strings, UEFI variables
- Overflow checking arithmetics
- PE image loading with no UEFI Secure Boot conflict
- Plist configuration format parsing
- PNG image manipulation
- Text output and graphics output implementations
- XNU kernel driver injection and patch engine

Early history of the codebase could be found in [AppleSupportPkg](https://github.com/acidanthera/AppleSupportPkg) and PicoLib library set by The HermitCrabs Lab.

#### OcGuardLib

This library implements basic safety features recommended for the use within the project. It implements fast
safe integral arithmetics mapping on compiler builtins, type alignment checking, and UBSan runtime,
based on [NetBSD implementation](https://blog.netbsd.org/tnf/entry/introduction_to_µubsan_a_clean).

The use of UBSan runtime requires the use of Clang compiler and `-fsanitize=undefined` argument. Refer to
[Clang documentation](https://releases.llvm.org/7.0.0/tools/clang/docs/UndefinedBehaviorSanitizer.html) for more
details.

#### Credits

- Everyone who made the original OpenCorePkg. See the original credits [here](https://github.com/acidanthera/OpenCorePkg).

#### Discussion

This fork doesn't have it's own discussion forums. (Yet?) The forum links in the code are for the original OpenCore.
