## Camera Timestamp Check

This blueprint will check the timestamp overlays on your security cameras and send a notification if the timestamp is not within a specified range of the current time. This can help ensure that your camera's time is synchronized with your Home Assistant instance. A conversation agent is used to extract the timestamp from the camera image overlay. The blueprint supports multiple cameras and can notify you via a mobile app or Telegram.

By default, the blueprint uses the Google Generative AI agent to extract timestamps from camera overlays. However, you can configure a different conversation agent if desired. The extracted timestamp is expected to be in the format `YYYY-MM-DD HH:MM:SS`.

[![Import blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://github.com/rsiv/home-assistant/blob/main/blueprints/automation/camera-timestamp-check.yaml)

---

### Prerequisites

- Conversation agent integration (Google Generative AI by default, or another supported agent)
- Mobile app notifications or Telegram integration

---
