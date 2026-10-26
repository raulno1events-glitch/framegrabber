# Framegrabber

A working repository for modernizing the legacy Slamtec RPLIDAR frame-grabber while preserving scan acquisition and connection behavior.

## Upstream sources

- Main SDK: https://github.com/Slamtec/rplidar_sdk
- Legacy frame-grabber reference: https://github.com/Slamtec/rplidar_sdk/tree/99478e5fb90de3b4a6db0080acacd373f8b36869/app/frame_grabber
- Reference commit: `99478e5fb90de3b4a6db0080acacd373f8b36869`

## Important project notes

The upstream frame-grabber is a Windows native C++/WTL application. It is distinct from the separately supplied `.NET` executable, so its UI and integration paths must not be assumed interchangeable.

The SDK is distributed under BSD-2-Clause, while upstream demo applications (including the legacy frame-grabber) identify themselves as GPL-3.0. Preserve the original copyright and license headers when redistributing or modifying source. See upstream license files before publishing derived binaries.

## Modernization goals

- Keep the original RPLIDAR connection and scan workflow intact.
- Improve visual hierarchy, connection status, scan visualization, and configuration UX.
- Keep device communication separate from UI code.
- Document build requirements and validate on Windows with a connected device before claiming hardware support.

## Current status

This repository was initially empty. The source import and modernization are in progress; do not treat this README alone as a buildable application.
