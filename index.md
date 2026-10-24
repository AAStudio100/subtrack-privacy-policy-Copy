# SubTrack Privacy Policy

**Effective Date:** October 19, 2026  
**Last Updated:** October 24, 2026  
**Developer:** Awais Labs  
**Privacy Contact:** mawais2674@gmail.com

## 1. Introduction

Welcome to SubTrack.

SubTrack is a subscription and recurring-expense tracking application developed by Awais Labs. It helps users organize subscriptions, bills, recurring payment schedules, spending summaries, payment history, and optional reminders.
We respect your privacy and aim to be transparent about how your information is stored, used, and managed.
This Privacy Policy explains SubTrack's data practices, including local storage, optional exchange-rate requests, Android backups, notifications, and third-party software.

## 2. Information You Enter

SubTrack allows you to enter and manage information such as:

- Subscription and recurring-payment names
- Payment amounts and currencies
- Payment categories
- Billing frequencies and due dates
- Optional notes
- Payment status and manually recorded payment history
- Reminder preferences and scheduled reminder times
- Optional currency-conversion preferences

This information is provided by you when using the application's features.
SubTrack does not require you to create an account or provide bank account details, credit card numbers, or payment credentials.
SubTrack does not connect to your bank, initiate financial transactions, or automatically verify whether payments have been made.

## 3. How Your Information Is Stored and Used

SubTrack stores subscription information, payment records, and reminder preferences in a private SQLite database within the application's storage on your Android device.
SubTrack uses this information to:

- Display and manage subscriptions and recurring bills
- Calculate recurring spending totals and summaries
- Display spending insights and manually recorded payment history
- Track upcoming and overdue payments
- Schedule optional local payment reminders
- Calculate optional estimated currency-converted totals

### Optional Currency Conversion

SubTrack provides an optional feature called **Estimated Combined Monthly Total**, which is disabled by default.
If you enable this feature, SubTrack requests published currency exchange rates from the third-party Frankfurter service over an HTTPS connection.
The request uses a fixed EUR base currency and a predefined list of supported currencies.
The exchange-rate request does not include your subscription names, payment amounts, notes, payment history, or selected display currency.
SubTrack stores the following information locally in a separate SQLite database:

- Retrieved exchange-rate information
- Whether estimated conversion is enabled
- Your preferred display currency
- The last exchange-rate request-attempt timestamp

Exchange-rate refresh attempts are limited to once per UTC calendar day. Previously retrieved rates may remain available for estimates for up to 72 hours.
Currency-converted totals are estimates based on published reference exchange rates and may differ from rates available through banks or payment providers.
The reviewed application code does not transmit your entered subscription or payment-history records to a server operated by Awais Labs.
Eligible locally stored information may also be processed through Android Auto Backup, as described below.

## 4. Android Auto Backup

SubTrack supports Android Auto Backup.

When Android backup is enabled and available on your device, Android may include eligible SubTrack application data in a backup associated with your Google account.
This may include information stored in SubTrack's local databases, including:

- Subscription and recurring-payment details
- Payment amounts, currencies, categories, and notes
- Payment history
- Reminder preferences and application settings
- Locally cached exchange rates
- Currency-conversion settings and preferred display currency
- Exchange-rate request-attempt information

Android and Google's backup services manage this process according to the applicable device settings, backup mechanisms, and Google policies.
Backup availability, frequency, included information, and successful restoration are not guaranteed.
If you reinstall SubTrack or move to another Android device, eligible previously backed-up information may be restored.
Information deleted locally may still exist in an earlier Android-managed backup and could reappear following restoration.
You can manage available backup options through your Android device or Google account settings.
Awais Labs does not operate its own cloud backup or synchronization service for SubTrack.

## 5. Notifications and Reminders

SubTrack offers optional local notifications to remind you about upcoming recurring payments.
Reminders are disabled by default for individual payments and may be enabled by you.
When notifications are enabled, SubTrack may request Android notification permission.
Scheduled reminders may include the subscription name and payment amount.
Depending on your Android notification and lock-screen settings, this information may be visible on your device's lock screen or notification panel.
SubTrack's current application functionality uses locally scheduled reminders rather than developer-operated remote push notifications.
You can manage notification permissions and notification visibility through your Android device settings.

## 6. Third-Party Services and Software

SubTrack is developed using Expo and React Native and includes software components supporting Android functionality, local storage, networking, and notifications.

### Frankfurter Exchange-Rate Service

When you enable Estimated Combined Monthly Total, SubTrack connects to the Frankfurter exchange-rate service to retrieve currency reference rates.
Website: https://frankfurter.dev/
The request contains the currency information needed to retrieve rates. It does not include your entered subscription details, amounts, notes, or payment history.
Like other internet connections, the request involves network-level information needed to communicate with the service, which may include an IP address and technical request metadata.
Frankfurter states that it does not log personal data, IP addresses, or request URLs and describes the use of aggregate traffic statistics through its infrastructure. These statements are based on information published by the service provider.
Awais Labs does not control Frankfurter's infrastructure or independent data-handling practices.

### Firebase and Android Notifications

SubTrack includes Expo Notifications, whose Android dependencies include Firebase Cloud Messaging functionality.
SubTrack is configured to disable automatic Firebase Cloud Messaging initialization and Firebase Analytics collection through Android application configuration.
The application currently uses local notifications and does not intentionally request remote push-notification registration tokens.
The effect of these safeguards in the final Android release build, including any SDK-generated identifiers or network communications, remains subject to release verification.

### Other Software and Platform Services

The reviewed application source does not include a configured advertising platform, dedicated analytics service, or dedicated crash-reporting service.
Android, Google, and included software libraries may independently provide operating-system or supporting functionality, subject to their applicable practices.
The inclusion of third-party software does not necessarily mean that every capability provided by that software is active.

## 7. Information Sharing

Awais Labs does not operate a service that receives or sells your entered subscription or payment-history records.
The reviewed SubTrack application does not provide a feature that sends these records to advertisers or data brokers.
When optional currency conversion is enabled, SubTrack contacts Frankfurter to retrieve exchange rates. The request does not contain your entered subscription or payment-history records, although network-level information may be processed to deliver the request.
Android-managed backup may transfer eligible application data to Google's backup infrastructure, as described in Section 4.
The final release build and included software components will be reviewed to determine whether any additional data-processing disclosures are required.

## 8. Data Security

SubTrack stores its application records within Android's private application storage, which is subject to Android's application sandbox protections.
The application uses SQLite databases for local storage. The reviewed application configuration does not enable separate SQLCipher database encryption.
Android-managed backups are subject to Google's applicable backup security and encryption protections, which depend on the platform and device configuration.
Network requests to the Frankfurter exchange-rate service use HTTPS.
No digital storage, communication, or backup system can be guaranteed to be completely secure.
We recommend protecting your device with a secure screen lock and maintaining up-to-date device software.

## 9. Data Retention and Deletion

SubTrack stores subscription information and manually recorded payment history locally until it is changed or deleted through the application's available controls or the device's data-management features.
You can permanently delete an individual subscription within SubTrack. Doing so also deletes the manually recorded payment history associated with that subscription from the local database.
Archiving a subscription does not permanently delete it.
SubTrack currently does not provide a separate in-app function to delete all records simultaneously or to delete payment history independently.
You may remove the application's locally stored data through Android's application storage settings or by uninstalling SubTrack.
Clearing the application's data or uninstalling it also removes its locally stored exchange-rate cache and currency-conversion preferences, subject to possible subsequent restoration from an eligible backup.
Deleting local application data does not necessarily delete an earlier Android-managed backup. Information from an existing backup may subsequently be restored.
Because SubTrack does not currently provide a user account or developer-controlled cloud database, there is no SubTrack account to request deletion of.
If you have questions about data deletion, contact mawais2674@gmail.com.

## 10. Children's Privacy

SubTrack is intended as a general subscription and recurring-expense management tool and is not specifically designed for children.
SubTrack does not provide an account-registration feature and does not intentionally request children's personal information.

## 11. Changes to This Privacy Policy

Awais Labs may update this Privacy Policy when SubTrack's features, data practices, third-party services, or applicable requirements change.
When the policy is updated, the Last Updated date will be revised.
The latest version will be made available through the application's published Privacy Policy link.

## 12. Contact Us

For privacy-related questions, concerns, or requests, contact:

**Developer:** Awais Labs  
**Email:** mawais2674@gmail.com  
**Application:** SubTrack
