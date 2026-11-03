# A2 Beauty

[Open A2 Beauty](https://beauty.amiraliyaghouti.com) · Release 0.12.1

A2 Beauty connects customer booking, specialist schedules and salon management in independent salon workspaces. Customer records and follow-ups use the shared A2 CRM domain.

## Owner-approved branch workspaces

Owners can organize multiple salons, invite an existing salon and enter its workspace after its owner approves the access. Each branch keeps its own customers, appointments, CRM and finances. Its owner chooses the permissions, can change them later or disconnect the organization; the home owner cannot expand those permissions.

Delegated sessions are separate from the branch owner's account and depend on the home owner's current session. Old branch sessions close when a grant changes. The interface offers a return to the home salon after access is withdrawn, without exposing its password or granting the branch session owner authority. Invitations expire and can be revoked; they are not sent externally.

CRM, appointment notifications and scheduled marketing use the current branch grant. Revocation pauses scheduled campaign work from that delegated account. Internal campaign tasks already created remain recorded. Organization switching does not merge customer databases or confer platform access.

## Platform plans and subscription records

A separate management workspace organizes salon plans and subscription periods. Salon owners cannot turn themselves into platform operators. Authorized operators receive a private, expiring setup link and choose their own password; platform and salon sign-ins remain independent.

Plans can remain drafts with no price. An unset price cannot be activated, and changing a plan does not rewrite previously recorded subscription terms. Operators can record activation, renewal, suspension, resumption and cancellation with version checks and retained history. A salon owner sees only that salon's terms in their account.

These are administrative subscription records. They do not charge a card, certify payment or automatically cut off salon access when a period expires or is suspended. No production price or paid subscription has been configured.

## Collections and staff commissions

Authorized managers can issue appointment bills with discounts, record manual collections/refunds, configure a percentage or fixed commission for each specialist/service, and record settlements already made to staff. Commission is based on money collected for completed services after discounts/refunds. Bills keep their original rule, so later rate changes do not rewrite past calculations. A refund after settlement can leave a negative balance to carry forward; the application does not withdraw funds.

Financial events retain their history. Unpaid bills can be voided before any collection, repeated submissions do not duplicate money, and excess collections, refunds or settlements are rejected. Refund forms distinguish reducing a fee from returning money while the fee remains due. CRM links an authorized manager to the exact customer's bills; CRM access alone does not reveal financial amounts. Staff need an explicit grant to read only their own commission statement. Manual records are not verified gateway payments and do not transfer money.

## Managers for individual service lines

The salon owner can give a manager booking access to selected services. Appointment lists, totals, details, changes and return-customer selection follow that choice. New services do not silently expand access. Changing a manager's scope closes their old sessions; notifications also recheck the current service grant.

Owners can now opt service managers into CRM. A service selector keeps relationship stages, additional contacts, follow-ups, activity and appointment history within the selected service. The customer's primary name and phone remain shared. Search cannot reveal another service's contacts or private salon records. A line manager completes only their own tasks; salon-wide financial, marketing and administration access stays separate.

Bookings create the service association automatically. Authorized salon-wide CRM managers can attach an existing record to another service without copying its earlier contacts or tasks. Service managers can create prospects in their permitted context, while independent stage/version checks prevent one service from overwriting another. Inactive services retain authorized CRM history. Service campaign tasks are now attached to that service; a contact entered for one service does not establish salon-wide marketing consent.

CRM forms now remain open until their updated list is ready. If a response is lost after a save, the interface explains how to retry; the same unchanged submission reuses its recorded result instead of creating a duplicate. Delayed refreshes no longer discard the next customer-record click.

First-time customer accounts still use customer registration or an authorized salon-wide manager. The interface identifies the selected scope and prevents stale access forms from restoring older grants.

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

For 0.12, 155 Beauty tests and six shared Core tests passed without skips. New cases cover service isolation, contact search/privacy, independent stages, task assignments, scoped receipts, account-ID collision, campaign context, consent boundaries, inactive services, revoked authority and transactional rollback. Existing booking, financial, platform, profile, scheduling and notification backend suites also passed.

Fifty-two local service-CRM browser states and 44 existing service-booking states passed in light/dark at mobile and desktop widths. Tests exercised owner permission forms, service switching, shared identity, scoped contacts/tasks, record attachments and denied services. Screenshots were inspected, and the worker upgrade retained an unsaved draft. Repeatable migrations, restricted database permissions and the prior-source fallback were checked.

The 0.12.1 correction passed 56 local CRM states with delayed requests and intentionally lost responses. A committed contact request was retried with the same identity and command key and created only one record. Existing asynchronous-panel checks, malformed-response handling and the worker upgrade also passed.

The final 0.12.1 release passed 52 service-CRM browser states on the public HTTPS site in both themes and widths, without page errors or horizontal overflow. All 27 public assets matched the release package. The first live 0.12.0 check exposed the delayed-refresh issue described above; it was corrected and the complete live matrix rerun. No real financial event, external notification or customer record was used; bookings and CRM changes were confined to explicitly synthetic salons.

The 0.10 release separately passed 48 local platform states and four public login layouts. Authenticated platform flows were tested locally; the production operator account awaits owner setup and acceptance. Subscription prices remain unset. Automatic billing, access cutoff and external payment processing are not enabled.

Kavenegar template settings are available, but SMS transport and OTP login remain disconnected. Verified self-service account recovery remains unfinished. Real payment transport is not connected. Physical iOS/Android Push receipt and device GPU performance are not established by browser tests. Calendar files require manual import and do not synchronize later changes.

This repository contains public product notes only. Private application source, infrastructure configuration, keys and customer data are not published here. Validation records observed behavior, not a guarantee of availability, security or marketing results.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
