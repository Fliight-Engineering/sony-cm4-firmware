# Sony CM4 Firmware Releases

🔒 **Private Repository** - This repository contains firmware releases for the Sony CM4 camera integration system.

## Latest Release

**v1.1.1** - Released November 06, 2025

[📥 Download Latest Release](https://github.com/Fliight-Engineering/sony-cm4-firmware/releases/tag/v1.1.1) | [📋 View Changelog](https://github.com/Fliight-Engineering/sony-cm4-firmware/releases/tag/v1.1.1)

Size: 174M | SHA256: `d13fc4ccdafba567...`

## Automatic Updates

Devices automatically check for updates by fetching:
- Manifest: https://raw.githubusercontent.com/Fliight-Engineering/sony-cm4-firmware/main/manifest.json

**Authentication:** Devices use a GitHub fine-grained PAT stored in `/etc/sony-cm4/github-token.conf` for read-only access to this private repository.

## Manual Installation

**Note:** Manual downloads require GitHub authentication.

1. Generate a fine-grained PAT with read access to this repository
2. Download the latest `.rauc` bundle: 
   ```bash
   curl -L -H "Authorization: Bearer YOUR_TOKEN" \
     "https://github.com/Fliight-Engineering/sony-cm4-firmware/releases/download/v1.1.1/sony-cm4-v1.1.1.rauc" \
     -o sony-cm4-v1.1.1.rauc
   ```
3. Install via: `rauc install sony-cm4-v1.1.1.rauc`
4. Reboot to activate

## Compatibility

- Hardware: Sony CM4 (Raspberry Pi Compute Module 4)
- RAUC Version: 1.8+
- Minimum Version: v0.8.0
- Authentication: GitHub PAT required for downloads

## Security

This repository is private to protect firmware releases. Contact Fliight Engineering for access.
