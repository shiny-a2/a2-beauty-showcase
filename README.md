# A2 Beauty

[Open A2 Beauty](https://beauty.amiraliyaghouti.com) · Release 0.7.0

A2 Beauty connects customer booking, specialist schedules and salon management in independent salon workspaces. Customer records and follow-ups use the shared A2 CRM domain.

## Editable profiles, connected customer records

Customers, specialists and managers can update their own names and contact numbers. Authorized managers can correct permitted accounts, while team managers can update a specialist's public introduction without receiving private account details. Login identifiers and access grants have separate controls.

Profile changes update the booking-linked primary CRM contact and customer name together. Consent, additional contacts, lead ownership, stage and follow-ups are preserved; appointment service and price snapshots stay intact. Competing edits cannot silently overwrite newer changes, retries do not duplicate activity, and the interface offers a way to reload the latest profile. A saved phone number is not verified identity or new permission to contact someone.

## Connected daily workflows

Specialists remain visible as the customer directory grows. Time off is paginated and editable, with overlap and stale-edit checks; existing dates stay intact in the editor. Working-hour changes protect appointments already in progress and the preparation time reserved after a service.

Managers can rename and reorganize service categories while keeping their services. Notifications open the exact appointment, including cancellations. CRM shows recorded activities and finds customers through contact names or phone numbers entered with Persian or Arabic digits. Account holders can close their other sessions after confirming their password; the current session stays open and disconnected sessions lose their Push subscriptions.

## Designed for a beauty salon

The customer catalog now has original dimensional illustrations for makeup, nails, hair, lashes and skincare. A rose, pearl and lilac identity connects the welcome page, service cards, appointment summary and staff/manager workspaces. Nested categories inherit suitable artwork; unfamiliar services use a neutral mirror while the salon's actual names, prices and availability remain visible. The mobile category shelf keeps service discovery compact.

The real three-dimensional vanity uses rose lacquer and champagne metal. Finite welcome motion, illustration hover, button feedback and native-dialog transitions respond to interaction, respect reduced motion and keep keyboard actions immediate. Focus stays on the selected service, date or time after the catalog updates. The installable app icon matches the new identity.

## Marketing built around salon visits

Managers can plan internal follow-ups for service return visits, inactive customers, first-visit feedback, loyal customers and missed appointments. Each salon sets its service return intervals, inactivity threshold, loyalty threshold and contact cooldown. Audience previews exclude customers who have denied contact, opted out of campaign planning, already booked a future appointment, have an open follow-up or recently received a campaign task.

Campaigns start as drafts. Managers can preview the audience, choose an editable task template, run immediately, schedule once or weekly, pause and archive. Scheduled work rechecks eligibility and the responsible manager's access before creating canonical CRM tasks. A delayed weekly schedule catches up once; it does not replay every missed week. Existing CRM tasks remain available after a campaign is archived.

Campaign reports separate created tasks, completed tasks and unique customers with a subsequent booking. A later booking is not proof of campaign impact or revenue. Unknown contact consent is marked for review, never treated as permission to advertise. These campaigns organize internal team work; they do not send SMS, email or promotional Push.

The activity panel shows the salon's audit history and appointment, reminder and campaign queue counts. Owners can delegate marketing and activity-report access separately. Scheduling fixes suppress stale reminders after an appointment starts, handle concurrent cancellation safely and prevent a reproduced lock-order conflict between reminder processing and booking changes.

## A studio for the whole salon

Persian typography, right-to-left layouts, rose, pearl and lilac surfaces and dimensional controls connect the customer, specialist and manager panels. The welcome page includes a real three-dimensional vanity scene with demand rendering, reduced-motion handling and an illustration fallback.

The full Persian calendar supports the ninety-day booking horizon. Appointment filters, details and manual calendar-file downloads help organize visits. Customer search, linked CRM history, granular account access, password onboarding, the in-app inbox and optional browser Push are included. The installable web app provides home-screen guidance. Demonstrations are explicitly synthetic and send no external notifications.

## Validation and boundaries

For 0.7, 98 Beauty tests and six shared Core tests passed without skips. New coverage includes tenant and permission boundaries, competing edits, access changes while a request is waiting, repeat submissions and complete rollback when CRM synchronization fails. Existing booking, notification, scheduling and marketing backend suites also passed.

Local browser validation passed 116 states/journeys across light/dark and desktop/mobile: 52 profile and CRM states, 24 account states and forty booking journeys. Tests included keyboard focus, stale-edit recovery, a closed dialog receiving a late response and unusually long specialist text. The observed biography overflow and stale account heading were fixed. A browser upgrade from the previous app worker retained an unsaved draft.

After activation, all 52 profile and CRM states passed over public HTTPS in both themes and screen sizes. Anonymous access to all three profile routes was denied. Tests used isolated synthetic salons and actual HTTP/database operations, with no real customer appointment, payment or external message. Published assets matched the reviewed release. Earlier maintenance, access/notification and marketing browser evidence belongs to the preceding release and was not counted as rerun coverage here.

Kavenegar template settings are available, but SMS transport and OTP login remain disconnected. Verified account recovery, line-specific manager access, payment processing, subscription billing, commission settlement, multi-branch chains and platform-wide administration remain future work. Current manager permissions apply across their salon. Physical iOS/Android Push receipt and device GPU performance are not established by browser tests. Calendar files require manual import and do not synchronize later changes.

This repository contains public product notes only. Private application source, infrastructure configuration, keys and customer data are not published here. Validation records observed behavior, not a guarantee of availability, security or marketing results.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
