# gl502vm-fx502vm-opencore-ventura
macOS 13 (Ventura) Hackintosh OpenCore config for ASUS GL502/FX502 series (飞行堡垒)

## Supported Hardware
`Many other models with similar hardware combo based on the same motherboard could work in theory. No support is given.`

ASUS FX502VM

i7 7700HQ

GTX 1060 3G

16GB RAM/512GB NVMe/1TB SATA HDD

BCM94331CSAX with Adapter

macOS 13.0.1 Ventura

## How to use

After initial set-up, generate new set of serial with your preferred OpenCore config.plist configurator, and patch NVIDIA WebDriver with [OpenCore Legacy Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher).

You might need to inject USB Ports again based on your hardware (mine came without the USB-C soldered), use a different set of wireless driver (you will need AirportItlwm and IntelBluetoothFirmware without hardware modifications), or make your own CPUFriend (if you has a CPU model other than 7700HQ).

Refer to the [Dortania Guides](https://dortania.github.io/getting-started/) for support.

## What isn't working and won't be fixed

Graphics bugs (no metal support and minor issues with GPU rendering): please wait for OCLP team's hard work

Backlight/brightness control: might work under 10.13 HS. No support for OCLP patched graphics for now as I haven't figured out a way to inject the EDID.

AWDL if you are not using a native Broadcom wireless/bluetooth chipset.
