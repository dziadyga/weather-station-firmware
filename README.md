# Weather Station Firmware

Firmware binaries and versioning for the ESP32-C3 Weather Station OTA updates.

## Directory Structure

- `firmware/` - Contains firmware binaries and version information
  - `version.txt` - Current firmware version
  - `firmware.bin` - Compiled firmware binary for OTA updates

## Workflow

1. Update firmware version in weather-station project config.h
2. Build and test locally
3. Copy compiled binary to `firmware/firmware.bin`
4. Update `firmware/version.txt` with new version number
5. Commit and push to GitHub
6. Device will auto-update on next boot if version is newer
