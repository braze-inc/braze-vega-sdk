## 0.3.0
- Updated `@braze/javascript-sdk` to 0.3.0, which fixes rate-limiting issues. See the [JavaScript SDK changelog](https://github.com/braze-inc/braze-javascript-sdk/blob/main/CHANGELOG.md) for the full list of changes.

## 0.2.0

##### ⚠️ Breaking
- Updated `@braze/javascript-sdk` to 0.2.0, which updates In-App Message constructors to take a single object as opposed to a large list of parameters. See the [JavaScript SDK changelog](https://github.com/braze-inc/braze-javascript-sdk/blob/main/CHANGELOG.md) for the full list of changes.
- The Braze Vega SDK now uses `MMKV` storage instead of `AsyncStorage` for better performance. To optionally clear AsyncStorage of Braze items, you can remove keys that start with `ab.`.

##### Fixed
- Fixed an issue where the `react-native-url-polyfill` package used by the Braze SDK could cause issues with Shaka player.

## 0.1.0

##### ⚠️ Breaking
- `initialize()` now returns a promise. This promise resolves to a boolean that indicates whether the initialization was successful. You must await/resolve this promise before calling other Braze methods.

##### Added
- Introduced support for triggering In-App Messages, as well as the following methods:
  - `addToCustomUserAttributeArray`
  - `deferInAppMessage`
  - `addUserAlias`
  - `addUserToSubscriptionGroup`
  - `deferInAppMessage`
  - `disableSdk`
  - `enableSdk`
  - `getDeferredInAppMessage`
  - `getDeviceId`
  - `handleBrazeAction`
  - `incrementCustomUserAttribute`
  - `isDisabled`
  - `logInAppMessageButtonClick`
  - `logInAppMessageClick`
  - `logInAppMessageHtmlClick`
  - `logInAppMessageImpression`
  - `logPurchase`
  - `removeAllSubscriptions`
  - `removeFromCustomUserAttributeArray`
  - `removeSubscription`
  - `requestImmediateDataFlush`
  - `setCustomUserLocationAttribute`
  - `setLogger`
  - `setUserDateOfBirth`
  - `setUserEmailNotificationSubscriptionType`
  - `setUserGender`
  - `setUserHomeCity`
  - `setUserLastKnownLocation`
  - `setUserPhoneNumber`
  - `setUserPushNotificationSubscriptionType`
  - `subscribeToInAppMessage`
  - `toggleLogging`
  - `wipeData`

## 0.0.2

##### Added
- Introduced the following methods:
  - `setUserFirstName`
  - `setUserLastName`
  - `setUserEmail`

## 0.0.1

- Initial release of the Braze Vega SDK with core functionality
- Includes the following methods:
  - `initialize`
  - `destroy`
  - `addUserAlias`
  - `addUserToSubscriptionGroup`
  - `changeUser`
  - `getUserId`
  - `logCustomEvent`
  - `openSession`
  - `removeUserFromSubscriptionGroup`
  - `setCustomUserAttribute`
  - `setUserCountry`
  - `setUserLanguage`
