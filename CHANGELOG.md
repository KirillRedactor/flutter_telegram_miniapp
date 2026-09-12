# Changelog

## 0.1.2

* Implemented support for **Bot API 10.1**
    * Added the field *chat_join_request_query_id* to the class [WebAppInitData](https://core.telegram.org/bots/webapps#webappinitdata).

## 0.1.1

* Implemented support for **Bot API 9.6**
    * Added the method *requestChat* to the class [WebApp](https://core.telegram.org/bots/webapps#initializing-mini-apps).

* Implemented support for **Bot API 9.5**
    * Added the field *iconCustomEmojiId* to the class [BottomButton](https://core.telegram.org/bots/webapps#bottombutton).

## 0.1.0

* **Breaking:** Unified the asynchronous API. The callback-based methods and their `*Async` counterparts have been merged into single `Future`-returning methods (e.g. `setItem`, `getItem`, `getItems`, `removeItem`, `removeItems`, `getKeys`, `showPopup`, `openInvoice`, `requestContact`, `init`, `requestAccess`, `authenticate`, `updateBiometricToken`).
* **Breaking:** Errors reported by the Telegram client are no longer silently ignored. Failing methods now complete with a `TelegramMiniAppException` instead of returning a default value.
* Added the `TelegramMiniAppException` class to the public API.
* Exported the `DeviceStorage` and `SecureStorage` types.
* Raised the minimum Dart SDK constraint to `^3.12.2`.
* Reformatted the codebase and refreshed the example and documentation to use the new async API.

## 0.0.12

* Fixed error with `haptic_feedback` with `impactOccurred` and `notificationOccurred` (Issue [#18](https://github.com/KirillRedactor/telegram_miniapp/issues/18))

## 0.0.11

* Fixed error with SafeAreaInset and ContentSafeAreaInset

## 0.0.10

* Implemented support for **Bot API 9.1**
    * Added the method *hideKeyboard* to the class WebApp.
* Fixed an error during static analysis

## 0.0.9

* Fixed an error in exporting enums

## 0.0.8

* Implemented support for Bot API 9.0
* Implemented DeviceStorage and SecureStorage
* Fixed error with authDate in initDataUnsafe

## 0.0.7

* Fixed a critical error with number conversion 

## 0.0.6

* Fixed a critical error in the event handler
* Added documentation for BackButton, BottomButton, CloudStorage, ContentSafeAreaInset, HapticFeedback, LocationData, LocationManager, MainButton.
* Fixed other minor bugs

## 0.0.5

* Fixed little problem

## 0.0.4

* Removed package 'async' from pubspec.yaml
* Fixed some problems

## 0.0.3

* Fixed some problems

## 0.0.2

* Added example project

## 0.0.1

* Repository inited
