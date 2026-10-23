# Doorbell Overlay 0.3.0

- Individual settings for Trigger 1 (Detection) and Trigger 2 (Doorbell Ring):
  - Dedicated camera size percentages for detection (e.g. 50% PIP) and doorbell ringing (e.g. 90% large popup).
  - Dedicated display durations for each event (e.g. 15s for detection, 30s for ring).
  - Dedicated overlay positions (Top, Top left, Top right, Center, Bottom, Bottom left, Bottom right).
  - Dedicated camera visibility/opacity settings.
  - Dedicated overlay labels (e.g. "Person detekteret" and "Dørklokke", or custom text; leave empty to hide badge).
  - Optional secondary camera entity for Trigger 2 if using different angles/streams.
- Instant seamless upgrade from detection preview to doorbell ring view when a visitor rings the bell while detection is already showing.
- Doorbell ring overlay is protected from being downgraded by background motion/person detection.
- Cached camera frame renders instantly on trigger, eliminating blank popup delays.
- Dedicated test commands for both detection (`showDetectionTest`) and doorbell ring (`showCameraTest`) events.
