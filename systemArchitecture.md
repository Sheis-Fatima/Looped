# System overview 
Looped is a cross-platform mobile application designed for students to stay informed, connected, and engaged.
It uses a client–server model built with Flutter on the frontend, Node.js on the backend, and Firebase as the core infrastructure for real-time data, authentication, and notifications.

# System build
**Frontend**
1. Framework: Flutter (Dart)
2. UI Toolkit: Material Design(Android), Carpertino Design(IOS)
3. State Management: Provider
4. API Communication: HTTP / Dio 

**Backend**
1. Language: JavaScript / TypeScript
2. Framework: Node.js with Express.js
3. API Architecture: RESTful API
4. Hosting: Render / AWS / Google Cloud Platform

**Database**
1. Primary Database: Firebase Firestore
2. Alternative Option: MongoDB
3. Hosting: Firebase Cloud or MongoDB Atlas.

**Authentication & Security**
1. Firebase Authentication
2. JWT (JSON Web Tokens)
3. Firebase Security Rules

**Notifications & Messaging**
1. Firebase Cloud Messaging (FCM)
2. Socket.io

**Storage & Media**
1. Firebase Storage
2. Cloudinary

**Calendar & Scheduling**
1. Packages
2. Automation

**Hosting & Deployment**
1. Backend Hosting: Render / AWS / Google Cloud Platform.
2. Database Hosting: Firebase Firestore / MongoDB Atlas.
3. Mobile App Deployment: Google Play Store and Apple App Store.

**Development Tools**
1. Version Control: Git + GitHub (public repository).
2. IDE: Visual Studio Code / Android Studio.
3. Design & Prototyping: Figma (for UI/UX wireframes and mockups).
4. Testing: Flutter Test / Postman (API testing).

# How components work
When a user logs in with their verified school email or OTP, Firebase Authentication confirms their identity and gives them secure access. The Flutter app then talks to the Node.js backend through safe API calls to fetch verified updates, events, and community information stored in Firebase Firestore.
Whenever a new event, post, or reminder is created, the backend triggers Firebase Cloud Messaging (FCM) to send real-time notifications directly to the user’s phone.
Media like photos or event banners are uploaded to Firebase Storage or Cloudinary, and all updates sync instantly across devices.

# Why the approach is technically feasible
It is designed to grow easily and stay reliable. Each part of the app, login, feeds, events, and chat can be improved without breaking anything else. It keeps students’ data safe with secure login and tokens, while updates and notifications show up instantly. Built with Flutter, Looped works smoothly on both Android and iOS, and its flexible design makes it easy to add new features in the future, like a web version or admin panel.
