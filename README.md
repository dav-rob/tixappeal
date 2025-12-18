# Tix Appeal

This meta-repository is the entry point for the Tix Appeal platform.

## Repositories

- 🌐 [Mobile App](https://github.com/dav-rob/tixapp-appeal-ai-smart)
- 🧠 [Legal Rules](https://github.com/dav-rob/tixapp-legal-rules)
- 🗂️ [Legal Data Model](https://github.com/dav-rob/ticket-adventure)
- 🧾 [OCR API](https://github.com/dav-rob/extract-ticket-data)
- ☁️ [Cloud Infrastructure](https://github.com/dav-rob/tixapp-deployment)
- ⚙️ [Rule Generation](https://github.com/dav-rob/tixapp-rule-generation)
- 🔍 [Tribunal Case Search](https://github.com/dav-rob/tixapp-tribunal-data)

## Architecture
```
Mobile App (iOS / Android)
  ├─ Auth via Google / Apple
  ├─ Ticket upload → OCR API (on shared Cloud Infrastructure)
  │     └─ Extracted data → Legal Rules API (on shared Cloud Infrastructure)
  │             └─ Drives navigation & progress using Legal Data Model
  │             └─ Rules traceability maintained via Rule Generation repo
  └─ High-value add-on: Tribunal Case Search (find similar tribunal outcomes)
```
