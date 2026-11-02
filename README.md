# A2 Beauty

[Open A2 Beauty](https://beauty.amiraliyaghouti.com) · Release 0.6.0

A2 Beauty connects customer booking, specialist schedules and salon management in independent salon workspaces. Customer records and follow-ups use the shared A2 CRM domain.

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

For 0.6, 88 Beauty tests and six shared Core tests passed without skips. Coverage includes tenant and permission boundaries, booking conflicts, ongoing appointments, concurrent edits, category cycles/depth, pagination beyond previous limits, CRM contact search, session revocation and subscription cleanup, reminder retries and marketing execution. A synthetic 5,000-contact search-plan check was also performed; it is not a production load benchmark.

Local browser validation passed 207 states/journeys across light/dark and desktop/mobile: 44 maintenance and integration states, 24 account states, 52 access/notification states, 47 marketing states and forty booking journeys. The real notification worker delivered synthetic booking changes to the in-app inbox. A browser upgrade from the previous app worker retained an unsaved draft. Interactive layouts and focus were inspected in both themes and sizes.

After activation, 44 maintenance/integration states passed over public HTTPS across both themes and screen sizes, plus ten booking journeys covering management, customer booking, rescheduling, specialist visibility and linked CRM history. Tests used isolated synthetic salons and the actual in-app notification worker, with no real appointment, payment or external message. Published assets matched the reviewed release.

Kavenegar template settings are available, but SMS transport and OTP login remain disconnected. Payment processing, subscription billing, commission settlement, multi-branch chains and platform-wide administration remain future work. Physical iOS/Android Push receipt and device GPU performance are not established by browser tests. Calendar files require manual import and do not synchronize later changes.

This repository contains public product notes only. Private application source, infrastructure configuration, keys and customer data are not published here. Validation records observed behavior, not a guarantee of availability, security or marketing results.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
