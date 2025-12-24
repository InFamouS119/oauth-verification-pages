# Google OAuth Verification Information

## App Details

**App Name**: OnlineStore
**Package Name**: com.infamous.onlinestore
**Project ID**: onlinestore-832f0
**Application Type**: Production (Not for Development/Testing/Staging use only)
**Usage Type**: Commercial/Public (Not for personal use only)

## OAuth Configuration

### OAuth Client IDs

- **Web Client ID**: 345633554088-sb6g3cebbgo3baearsm8tc8dapq4oeav.apps.googleusercontent.com
- **Android Client ID**: 345633554088-sb6g3cebbgo3baearsm8tc8dapq4oeav.apps.googleusercontent.com

### SHA-1 Fingerprints

- **Debug**: 17:E7:5A:4A:B4:C8:3B:18:B4:83:9F:FF:65:F3:86:B8:6F:24:3A:48
- **Release**: 96:CB:54:42:97:9F:A5:29:D8:8D:5D:47:9E:C3:A3:B7:15:54:BB:8D

## Test Account Credentials

### Primary Test Account
- **Email**: test@example.com
- **Password**: TestPass123!

### Alternate Test Account
- **Email**: test2@example.com
- **Password**: TestPass456!

## OAuth Scopes Requested

1. **email** - To retrieve the user's email address
2. **profile** - To retrieve the user's basic profile information
3. **openid** - To authenticate the user

## Authentication Flow

1. User taps "Sign in with Google" button
2. Google OAuth consent screen is displayed
3. User selects account or enters credentials
4. User grants requested permissions
5. App receives authentication token
6. User profile is created/updated in Firestore
7. User is redirected to app home screen

## Firebase Integration

### Firebase Project
- **Project ID**: onlinestore-832f0
- **Firebase Auth**: Enabled with Google provider
- **Firestore Database**: Used for user profile storage

### User Data Storage
User profiles are stored in the `users` collection in Firestore with the following structure:
```json
{
  "id": "user_uid",
  "name": "User Name",
  "email": "user@example.com",
  "profileImage": "https://example.com/image.jpg",
  "username": "username",
  "phone": "+1234567890",
  "country": "United States",
  "address": "123 Main St",
  "address2": "Apt 4B",
  "createdAt": "timestamp",
  "lastLoginAt": "timestamp"
}
```

## App Features Accessible via OAuth

1. **User Profile Management**
   - View and edit profile information
   - Upload profile picture
   - Update contact details

2. **Product Browsing**
   - Browse product categories
   - Search products
   - View product details

3. **Shopping Cart**
   - Add/remove items
   - Update quantities
   - Proceed to checkout

4. **Order Management**
   - View order history
   - Track order status
   - Manage returns

5. **Wishlist**
   - Save favorite products
   - Organize wishlist items

6. **Notifications**
   - Receive promotional offers
   - Order status updates
   - Product availability alerts

## Security Measures

1. **Token Storage**: Authentication tokens are securely stored using React Native AsyncStorage
2. **Data Encryption**: All user data is encrypted in transit and at rest
3. **Session Management**: Automatic session timeout after 24 hours of inactivity
4. **Account Verification**: Email verification required for new accounts

## Privacy Policy

Our privacy policy is available at: https://example.com/privacy-policy

Key points:
- We only collect data necessary for app functionality
- User data is never sold to third parties
- Users can request data deletion at any time
- We comply with GDPR and CCPA regulations

## Support Contact

For any verification questions, please contact:
- **Email**: support@example.com
- **Phone**: +1 (555) 123-4567

## Additional Notes

1. The app is built using React Native Expo framework
2. All OAuth flows are handled through Firebase Authentication
3. No sensitive scopes are requested beyond basic profile information
4. Test accounts have been pre-populated with sample data for review
5. The app follows all Google OAuth best practices and security guidelines
6. **This is a production application intended for public use, not for development/testing/staging only**
7. **This is a commercial application for public use, not for personal use only**
8. **The source code is not currently hosted in a public repository**

## Screenshots

Relevant screenshots showing the OAuth flow are available in the app store listing and can be provided upon request.