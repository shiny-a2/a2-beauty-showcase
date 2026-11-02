# A2 Beauty

[Open A2 Beauty](https://beauty.amiraliyaghouti.com) · Release 0.2.0

A2 Beauty connects customer booking, specialist schedules and salon management in independent salon workspaces. Customers choose nested services and an available specialist; booking connects to the shared A2 CRM domain for customer records and follow-ups.

Version 0.2.0 lets the salon owner create manager, staff and customer accounts, set initial passwords and choose each account's access. A delegated manager cannot grant more authority than they hold or change the owner. New and reset passwords must be changed on first login. Access and password changes close prior sessions.

An in-app inbox now shows appointment creation, changes, cancellation and reminders. Browser Push is available with the user's permission and an active session. The installable web app includes notification navigation and home-screen guidance. A personal-device login option keeps the session for thirty days; logging out disconnects that session's Push subscription.

The interface is Persian and right-to-left, with Jalali dates, light/dark themes and mobile/desktop layouts. The earlier panel audit is included: CRM pagination and search, inactive-service administration, customer-aware availability, original-duration rescheduling and private-session cleanup have been corrected. The marked demonstration remains synthetic and sends no external notifications.

## Validation

Thirty-five Beauty tests and six shared Core tests passed locally. Coverage includes tenant boundaries, delegated-access denial, password onboarding, schema upgrade, concurrent booking, outbox/inbox idempotency, Push retry/expiration and session revocation. Forty existing browser journeys, 52 access/notification states and sixteen account-onboarding states passed across four desktop/mobile and light/dark combinations. The new screens were inspected for overflow and interactive states.

The HTTPS release, migration, application permissions and synthetic booking-to-inbox flow were verified after deployment. Push transport tests used mocks, and encryption/VAPID configuration was validated without sending a message. Actual notification receipt on a physical iOS/Android device remains an acceptance check; provider acceptance is not proof of device delivery.

## Release scope

Kavenegar template names can be prepared for login, appointment updates/reminders and verified payment. SMS sending and OTP login are deliberately disconnected. Payment processing, subscription billing, commission settlement, multi-branch chains and a platform-wide administration console are not enabled.

This repository contains public product notes only. Application source, infrastructure configuration, keys and customer data remain private. These checks describe tested behavior, not a guarantee of availability or security.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
