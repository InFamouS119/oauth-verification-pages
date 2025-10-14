# Scripts for OnlineStore Application

This directory contains various scripts for managing the OnlineStore application.

## Available Scripts

### 1. Create Test User
Creates a test user account for Google Play review process.

```bash
npm run create-test-user
```

This script creates a test user with the following credentials:
- Email: test@example.com
- Password: TestPass123!

The account is fully functional and can be used to review all app features.

### 2. Initialize Firestore Collections
Initializes Firestore collections with sample data.

```bash
node initialize-firestore-collections.js
```

### 3. Migrate User Data
Migrates user data from one format to another.

```bash
npm run migrate-users
```

## Firebase Admin SDK Setup

All scripts use the Firebase Admin SDK with the service account key located at:
`../onlinestore-832f0-firebase-adminsdk-fbsvc-7300134834.json`

Make sure this file is present and has the correct permissions.

## Test Account for Google Review

For Google Play app review, use the following test account credentials:
- Email: test@example.com
- Password: TestPass123!

This account has full access to all app features and no real personal information is associated with it.