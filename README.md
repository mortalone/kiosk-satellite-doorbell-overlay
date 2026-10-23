# Doorbell Overlay

Doorbell camera overlay for Kiosk Satellite screensavers and Fotoo with dual Home Assistant triggers, aspect-safe camera sizing, and individual event configuration.

Install in **Kiosk Satellite → Plugin Manager → Add plugin** using this repository URL:

`https://github.com/mortalone/kiosk-satellite-doorbell-overlay`

## Main features

- **Dual event triggers**: Trigger 1 for detection (e.g. Frigate person occupancy) and Trigger 2 for doorbell ring (e.g. Reolink visitor button).
- **Individual event settings**:
  - Independent camera size (e.g. compact 50% PIP stream for person detection, large 90% view when doorbell rings).
  - Independent display time (e.g. 15s for detection, 30s for doorbell ring).
  - Independent positioning (Top, Top left, Top right, Center, Bottom, Bottom left, Bottom right).
  - Independent opacity and custom overlay labels (or hide label entirely).
  - Optional secondary camera entity for Trigger 2.
- **Smart prioritization**: Doorbell ring immediately upgrades an active detection overlay and cannot be downgraded by background motion.
- **Instant frame rendering**: Pre-rendered cached camera frames show immediately without network latency.
- Uses the in-Activity overlay path on Kiosk Satellite and the system overlay on Fotoo.

## Notes

Do not enable this standalone Doorbell plugin at the same time as the doorbell part of the old combined Screensaver Overlay, or duplicate camera overlays may appear.
