<p align="center">
  <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779241423/%E0%B8%AA%E0%B8%81%E0%B8%A3%E0%B8%B5%E0%B8%99%E0%B8%8A%E0%B9%87%E0%B8%AD%E0%B8%95_2026-05-20_084327_qaqnhc.png" width="220"/>
  <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779241693/%E0%B8%AA%E0%B8%81%E0%B8%A3%E0%B8%B5%E0%B8%99%E0%B8%8A%E0%B9%87%E0%B8%AD%E0%B8%95_2026-05-20_084806_arsa4m.png" width="220"/>
  <img src="https://res.cloudinary.com/dpa96jvla/image/upload/v1779241747/%E0%B8%AA%E0%B8%81%E0%B8%A3%E0%B8%B5%E0%B8%99%E0%B8%8A%E0%B9%87%E0%B8%AD%E0%B8%95_2026-05-20_084858_se4vfw.png" width="165"/>
</p>

## Example Flex Message (JSON)

Below is an example of a Flex Message used in this system for healthcare communication via LINE Messaging API.

```json
{
  "type": "bubble",
  "hero": {
    "type": "image",
    "url": "https://res.cloudinary.com/ds6xq6wbm/image/upload/v1756009686/%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3.png",
    "size": "full",
    "aspectRatio": "20:13",
    "aspectMode": "cover"
  },
  "body": {
    "type": "box",
    "layout": "vertical",
    "contents": [
      {
        "type": "text",
        "text": "Telemedicine",
        "weight": "bold",
        "size": "xl"
      },
      {
        "type": "text",
        "text": "บริการปรึกษาแพทย์ทางไกล",
        "wrap": true,
        "margin": "md"
      }
    ]
  }
}
```
## Notes

Built 11+ Flex Messages using the LINE Messaging API free tier.

## Project Reference

LinkedIn:
https://www.linkedin.com/posts/ratchanon-noknoy_softwareengineering-backendengineering-systemsthinking-share-7437740581310648320-BKiJ
