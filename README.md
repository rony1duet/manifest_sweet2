# manifest_sweet2

Local manifest repository for compiling PixelOS on Redmi Note 12 Pro 4G (`sweet2`).

## Target Branch: Android 17 (`PixelOS-17-base`)

Includes:
- Device trees: `android_device_xiaomi_sweet2` & `android_device_xiaomi_sm6150-common` (`PixelOS-17-base`)
- Kernel: `android_kernel_xiaomi_sm6150` (`PixelOS-17-base`)
- Vendor: `android_vendor_xiaomi_sweet2` & `android_vendor_xiaomi_sm6150-common` (`PixelOS-17-base`)
- Hardware: `android_hardware_xiaomi` & `hardware_dolby` (`PixelOS-17-base`)
- Prebuilts & GCam: `android_prebuilts_sweet2` & `GCam_sweet2` (`PixelOS-17-base`)
- Build Soong: `android_build_soong` (`seventeen`)

## Usage

Clone into your ROM workspace before syncing:

```bash
git clone https://github.com/rony1duet/manifest_sweet2.git .repo/local_manifests -b PixelOS-17-base
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
