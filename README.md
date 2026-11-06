# manifest_sweet2

Local manifest repository for compiling PixelOS on Redmi Note 12 Pro 4G (`sweet2`).

## Target Branch: Android 16 (`PixelOS-16-QPR2`)

Includes:
- Device trees: `android_device_xiaomi_sweet2` & `android_device_xiaomi_sm6150-common` (`PixelOS-16-QPR2`)
- Kernel: `android_kernel_xiaomi_sm6150` (`PixelOS-16-QPR2`)
- Vendor: `android_vendor_xiaomi_sweet2` & `android_vendor_xiaomi_sm6150-common` (`PixelOS-16-QPR2`)
- Hardware: `android_hardware_xiaomi` & `hardware_dolby` (`PixelOS-16-QPR2`)
- Prebuilts & GCam: `android_prebuilts_sweet2` & `GCam_sweet2` (`PixelOS-16-QPR2`)
- Uses standard upstream `build/soong` (`sixteen-qpr2`)

## Usage

Clone into your ROM workspace before syncing:

```bash
git clone https://github.com/rony1duet/manifest_sweet2.git .repo/local_manifests -b PixelOS-16-QPR2
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
