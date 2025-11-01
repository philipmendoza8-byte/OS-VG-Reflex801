# VG LocalSystem Patch v2.2 — Auto-Verify + Disk Clean

**Date:** 2025-11-01  
**Custodian:** philipmendoza8-byte  
**Linked Repo:** [OS-VG-รีเฟล็กซ์801](https://github.com/philipmendoza8-byte/OS-VG-Reflex801)

## Overview
System upgrade for Reflex801 (macOS)
- Auto-Verify checksum (SHA256) after each sync
- Automatic cleanup of empty directories in `/RAW`
- Dual backup path: exHDD (`/Volumes/VG801/Backups`) + Google Drive (`vg.reflex801@gmail.com`)
- LaunchAgent automation (`com.vg.rawsync.watch.plist`)

## Patch Summary
| Function | Status | Note |
|-----------|--------|------|
| Auto-Verify SHA256 | ✅ | Matched checksum verified |
| Disk Clean | ✅ | Safe delete of empty subfolders only |
| Drive Sync | ✅ | Synced to both Drive & exHDD |
| LaunchAgent | ✅ | Auto reload confirmed |

## Changelog
- Added verification after archive
- Added log path isolation in `/LOGS`
- Optimized launchctl reloading behavior

---

**Next Milestone:** v2.3 — “Auto-Restore + Notification Layer”
