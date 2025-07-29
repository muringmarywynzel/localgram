# localgram

# 📱 LocalGram – Offline-First Social Media iOS App

**LocalGram** is a simple offline-first social media-style iOS app built using Swift and Core Data (or SQLite). Designed as a pet project for iOS developers, it demonstrates how to build a functional social feed entirely using local data persistence.

---

## ✨ Features

- 📝 Create posts with text and/or image
- ❤️ Like/unlike posts
- 🗑️ Edit or delete posts
- 📰 View posts in a timeline feed (most recent first)
- 💾 Offline-first with local persistence using Core Data or SQLite

---

## 📸 Screenshots

*(Add screenshots here of the feed, post creation, and like interaction)*

---

## 🧱 Architecture

**Pattern:** MVVM (Model-View-ViewModel)

- `Model`: Core Data Entity (`Post`)
- `ViewModel`: Business logic and interaction with Core Data
- `View`: SwiftUI (or UIKit) interface rendering the feed, post creation form, etc.

---

## 🗃️ Core Data Model

**Entity: `Post`**

| Field        | Type        | Description                    |
|--------------|-------------|--------------------------------|
| `id`         | UUID        | Unique identifier              |
| `contentText`| String?     | Optional text content          |
| `imageData`  | Binary Data | Optional image in Data format  |
| `createdAt`  | Date        | Timestamp of post creation     |
| `isLiked`    | Bool        | Like toggle (default: false)   |

---

## 🧩 Folder Structure
