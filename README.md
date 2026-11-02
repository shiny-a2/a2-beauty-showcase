# A2 Beauty

[Open A2 Beauty](https://beauty.amiraliyaghouti.com) · Release 0.5.0

A2 Beauty connects customer booking, specialist schedules and salon management in independent salon workspaces. Customer records and follow-ups use the shared A2 CRM domain.

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

For 0.5, forty booking journeys, 52 access/notification states, 47 marketing states and thirty new customer-experience states passed in light/dark and desktop/mobile. Eight final states checked service badges and selected/hovered navigation. Checks include narrow 320px layouts, artwork loading, nested-category fallback, keyboard focus, semantic text contrast and reduced motion. The graphics harness confirmed bounded pointer response, no idle drawing, cleanup and an illustration fallback. Two worker unit checks and a browser worker upgrade passed without losing the open draft. Browser results do not establish physical-device rendering performance.

After 0.5 activation, thirty customer-experience states passed over public HTTPS in both themes and screen sizes, plus ten end-to-end journeys covering salon management, customer booking, rescheduling, specialist visibility and linked CRM history. The checks used isolated synthetic salons, with no real appointment, payment or external message. Published assets matched the reviewed release.

For the 0.4 foundation, eighty Beauty tests and six shared Core tests passed locally. Coverage includes booking integrity, tenant and actor boundaries, permission revocation, stale reminders, concurrent cancellation, campaign idempotency, eligibility suppression, weekly catch-up, bounded retries, safe diagnostics, archival preservation, reporting and pagination. Forty existing booking journeys, 52 access/notification states, 47 integrated marketing states and a separate 64-state marketing review passed across desktop/mobile and light/dark. Eight final visual states checked the integrated activity and campaign layouts.

After the 0.4 activation, twenty public-HTTPS interface states passed across both themes and screen sizes. The actual timer processed one scheduled synthetic campaign and preserved its execution record after archival. It had zero eligible recipients and sent no messages. Public assets matched the reviewed release.

Kavenegar template settings are available, but SMS transport and OTP login remain disconnected. Payment processing, subscription billing, commission settlement, multi-branch chains and platform-wide administration remain future work. Physical iOS/Android Push receipt and device GPU performance are not established by browser tests. Calendar files require manual import and do not synchronize later changes.

This repository contains public product notes only. Private application source, infrastructure configuration, keys and customer data are not published here. Validation records observed behavior, not a guarantee of availability, security or marketing results.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
