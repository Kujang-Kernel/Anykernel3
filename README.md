# AnyKernel3 — Kujang Kernel

[![Telegram](https://img.shields.io/badge/Telegram-Kujang%20Project-2AABEE?logo=telegram&logoColor=white)](https://t.me/kujang_project)
[![Kernel](https://img.shields.io/badge/kernel-Kujang--Beta-orange)](https://github.com/Kujang-Kernel/Kujang_Kernel_Sweet)

AnyKernel3 flashable ZIP packer for **Kujang Kernel** on Redmi Note 10 Pro (`sweet` / `sweetin`).

## Supported devices

- `sweet` / `sweetin` — Redmi Note 10 Pro
- Android 11 – 17

## Notes

- Flash from recovery. Wipe cache before the first boot.
- Includes a **90 Hz DTBO selector**: in recovery, press **Volume Up** for the 90 Hz DTBO or **Volume Down** to keep the stock one (10 second timeout). If `dtbo-90hz.img` is missing, the stock DTBO is used automatically.
- The visible flash banner lives in the `banner` file and is printed by `META-INF/com/google/android/update-binary`.
- Kernel identity (`kernel.string`) is set in `anykernel.sh`.

## Build

The parent kernel builds the ZIP through `.github/workflows/Kujang_Beta.yml`, which clones this repository from branch `Kujang-Kernel`:

```sh
git clone --depth=1 -b Kujang-Kernel https://github.com/Kujang-Kernel/Anykernel3.git AnyKernel3
```

## Links

- Kernel source: [Kujang-Kernel/Kujang_Kernel_Sweet](https://github.com/Kujang-Kernel/Kujang_Kernel_Sweet)
- Community: [@kujang_project](https://t.me/kujang_project)

## Credits

- **osm0sis** — AnyKernel3
- **Kujang-Kernel** — device configuration and packaging
