# A2 Beauty

[Open A2 Beauty](https://beauty.amiraliyaghouti.com) · Release 0.3.1

A2 Beauty brings customer booking, specialist schedules and salon management into independent salon workspaces, with customer records and follow-ups connected to the shared A2 CRM domain.

## A studio for the whole salon

The interface has been redesigned around emerald and lilac surfaces, dimensional controls and a real three-dimensional vanity scene. Persian typography, right-to-left layouts, light/dark themes and responsive panels carry the same visual identity from the welcome page through customer, specialist and manager workspaces. The scene renders only when needed, honors reduced motion and retains an illustration when browser graphics are unavailable.

Customers can choose a date through the ninety-day booking horizon using a full Persian calendar. Appointment lists now include period, status, specialist, date-range and ordering filters. Details show the recorded appointment timeline, and confirmed appointments can be downloaded for manual import into a phone calendar. Later appointment changes do not automatically update that imported event.

Managers can search customers while booking, including long names and masked contact hints. CRM profiles include linked appointment history and visit summaries. Completed-service value is shown separately from money received. Access remains scoped to each salon, account role and assigned permissions.

Salon owners can create manager, staff and customer accounts, set initial passwords and choose capabilities. Initial and reset passwords must be changed before entering the panel. The in-app inbox and optional browser Push cover appointment events and reminders. The installable web app includes home-screen guidance and notification navigation. The clearly marked demonstration uses synthetic data and sends no external notifications.

## Validation

Forty-nine Beauty tests and six shared Core tests passed locally, including booking integrity, tenant and ownership boundaries, capability denial, customer search, CRM linkage, calendar handling and notification behavior. Browser checks covered forty existing booking journeys, 52 access/notification states, sixteen onboarding states and 48 new appointment-workspace states across mobile/desktop and light/dark. A further sixteen visual states checked the integrated calendar, filters, details and history, including readable selected-hover states.

After deployment, the 48 new appointment-workspace states passed again over public HTTPS using isolated synthetic salons, with no captured request failures, JavaScript errors or horizontal overflow. The deployed interface assets matched the reviewed release.

The graphics checks covered demand rendering, resource cleanup, reduced motion and unavailable WebGL. The built scene was also checked in the integrated application. These checks do not establish physical-device GPU performance or notification receipt on a particular iOS/Android device.

## Release scope

Kavenegar template names can be prepared for login, appointment updates/reminders and verified payment, but SMS sending and OTP login remain disconnected. Payment processing, subscription billing, commission settlement, multi-branch chains and platform-wide administration remain future work. Calendar files provide manual import, not synchronization.

This repository contains public product notes only. Application source, infrastructure details, keys and customer data remain private. Validation describes observed behavior, not a guarantee of availability or security.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
