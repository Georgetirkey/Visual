# Visual v2 — Python/Kivy Social App

Twitter-style social MVP with Firebase Realtime Database.

### Features
- Dark polished mobile UI
- Signup/login
- Home timeline
- Create posts
- Like/unlike posts
- Comment on posts
- Follow/unfollow users
- Search users
- Notifications for likes, comments and follows
- Verification application
- Admin verification queue
- Admin can approve as Blue, Blue+, Red or Gold
- Firebase role-based admin protection
- GitHub Actions APK build

### Setup
1. Firebase Console: enable Authentication > Email/Password.
2. Create/enable Realtime Database.
3. Import `firebase_database.rules.json`.
4. Push the repository to GitHub.
5. Actions → Build Visual APK → Run workflow.
6. Download the APK artifact.

### Security
The UI hides the admin navigation for normal users, but Firebase rules are the actual access control. For a production deployment, use Firebase App Check, stricter indexes/rules and server-side moderation/audit functions.

### Current MVP limitation
The UI uses text posts and Firebase REST directly. Image/video uploads, pagination, advanced profile pages, realtime listeners, push notifications and production-grade moderation should be added before public launch.
