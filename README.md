# Dark Bio - Ark Emulator Firmware Images

This repository contains the pre-built ArkOS images consumed by the [Ark Emulator](https://github.com/dark-bio/emulator). There is no code here, only release assets.

- The images are the emulator variant of the ArkOS firmware, built for QEMU's virtual hardware.
- The images are published automatically whenever a firmware version is promoted to **release**:
  - `arkos-X.Y.Z-COMMIT-emulator-kernel.ARCH`: Linux kernel for the QEMU guest.
  - `arkos-X.Y.Z-COMMIT-emulator-initrd.ARCH.gz`: ArkOS initramfs for the QEMU guest.
- The images are built for both `arm64` and `amd64` guests; the emulator bundles the build host's arch only.

*Note: The git tags in this repository version the published images, not any source code; the firmware itself is not public currently.*

## Usage

The emulator's release CI fetches the images pinned in its workflow and bundles them into the platform installers. Source builds of the emulator can download a release's kernel and initrd and pass them via `--kernel`/`--initrd`.

## Terms

The images are proprietary binaries of Dark Bio AG, published for use with the Ark Emulator. All rights reserved.
