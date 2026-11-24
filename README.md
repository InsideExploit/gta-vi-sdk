# gta-vi-sdk

C++ SDK of Grand Theft Auto VI (RAGE), dumped statically from the game executable with [gta-vi-dumper](https://github.com/InsideExploit/gta-vi-dumper).

Each folder is one game build:

| Build | Folder |
| --- | --- |
| 1.0.2.1 (Xbox Series) | [`1.0.2.1`](1.0.2.1) |

| File | Contents |
| --- | --- |
| `Basic.hpp` | RAGE core types (`atArray`, `atString`, `atHashString`, `Vec3V`, ...) with their x64 sizes. |
| `Enums.hpp` | Enums used by the parser structures. |
| `Classes.hpp` | Parser structures with their members at the registered offsets. |
| `Asserts.hpp` | Size and offset checks. Include it in one translation unit. |

Names are recovered by hash. A structure, member or enum whose name has not been recovered yet is written as its hash, `_0xXXXXXXXX`.