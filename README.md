# A2 Beauty

[Open the product catalogue](https://beauty.amiraliyaghouti.com) · [Sign in](https://beauty.amiraliyaghouti.com/login) · [Set up a salon](https://beauty.amiraliyaghouti.com/start)

Release **0.24.0** connects customer booking, specialist schedules and salon management in independent salon workspaces. Beauty uses the shared A2 CRM and loyalty engines for customer relationships and service points.

## A catalogue that follows your scroll

Version 0.24 keeps a three-dimensional beauty studio beside the product story. Scrolling through the introduction, Essential, Growth and Intelligence changes the studio angle, accessory positions and artwork while the feature text stays readable. Scrolling back restores earlier poses. Chapter links support the keyboard and show the current section.

The studio adapts to mobile, desktop and short landscape layouts. A Reduce motion control remembers the visitor's choice, and the device's reduced-motion setting takes precedence. If browser graphics are unavailable, an illustrated fallback remains. Rendering settles when input stops and pauses while the scene is out of view. Native scrolling, login links and the existing theme control remain available.

## Explore the product

The catalogue presents three groups of capabilities: **Essential**, **Growth** and **Intelligence**. These are feature chapters; they are not a promise of finalized subscription prices or automatic AI predictions.

Enter **visitor12** on the login page and leave the password empty to open an isolated, populated demo. Switch between manager, specialist and customer panels to explore related services, appointments, CRM records, marketing work, financial reports and loyalty gifts. A connected sample branch demonstrates permission-based access.

Demo names, contact details, prices and financial records are synthetic. Demo activity does not send external messages or transfer money, and each demo expires. It does not give access to an existing salon or platform administration. Ordinary accounts still require their credentials.

## Clear mobile navigation

Version 0.23 replaces the scrolling bottom bar with a few fixed destinations and a labeled menu button. Managers reach today's work, appointments, new bookings and customers directly. Specialists and customers receive shortcuts for their own daily tasks. The menu groups the remaining permitted sections, including finance, team, settings and account access.

The active section remains visible, closing the menu restores keyboard focus, and selecting a section opens its page. Version 0.23.1 groups the manager desktop sidebar into expandable salon work, customers, finance, administration and account sections. Daily work and the current page group open automatically. Keyboard users can expand or collapse each group; selecting a destination moves focus to its page heading. Short specialist and customer lists remain directly accessible. Navigation respects the same role, service-line and first-login restrictions as before; it does not grant new access.

## Follow up with the next customer

Version 0.22 opens CRM on a follow-up desk, with customer records one action away. Managers can filter open or completed work, past or upcoming due times and their own assignments. Each task names the customer and opens the related record. Completing a task uses the same shared CRM history; it does not send a message.

Filters collapse on the page so the work stays easy to reach on a phone. Dates display in Tehran time. Service-line managers still see only their permitted service and assigned work. The existing shared CRM engine remains the source of truth; this release adds no separate task database or marketing sender.

## Recover an account with a saved key

Version 0.21 adds private recovery keys for salon accounts and the separate platform administration account. While signed in, a user confirms their current password to prepare a key, saves it privately, and can replace or revoke it later. A key is displayed only when it is created. Recent recovery activity is visible in the account dialog.

If the password is forgotten, the login page accepts the account details and previously saved key to set a new password. A successful reset replaces the consumed key, closes existing sessions and removes that salon account's Push subscriptions. The user then signs in explicitly. Keys cannot recover a different account or salon, and demo/branch-delegated sessions cannot prepare them.

This requires preparation before losing access. Losing both the password and key still needs verified assisted recovery. It does not provide SMS/email recovery, automatic security messages or multifactor authentication.

## Safer account sign-in

Version 0.20 strengthens stored passwords through the shared A2 runtime. New passwords use the stronger format; an existing password is upgraded after a successful sign-in, without asking the user to choose a new password or closing their other valid sessions. Failed sign-in and concurrent password/access changes cannot overwrite a newer credential. The separate platform operator realm receives the same upgrade protection.

Password processing has a bounded queue. During saturation, salon and platform login forms explain when to retry. A compatible fallback release was verified before enabling stronger writes, so source rollback can still read upgraded credentials. Saved-key recovery is added in version 0.21; multifactor authentication remains pending.

## Privacy in operational logs

Version 0.19.1 minimizes new Beauty access records: query parameters and referrer information are omitted, including customer search terms. Response status and timing remain available for troubleshooting. Cookies, authorization headers and request bodies are not access-log fields. Existing records are unchanged; URL paths and other error-log conditions require separate review.

## Demo maintenance

Version 0.19 adds an explicit operator workflow for reviewing and removing old demo workspaces after their access period and an additional seven-day recovery grace. Cleanup preserves connected branch groups, excludes valid or permanent salons and requires a matching preview plus a backup before removal. The ordinary web service receives no extra deletion privileges. This is a maintenance command, not an automatic background purge; ongoing capacity checks and backup custody remain operational responsibilities.

## Essential — daily salon work

Owners can create a salon from the catalogue or login page, then follow setup tasks for specialists, services and prices, working hours and the salon address. Progress reflects current configuration: deactivating a specialist can make a service need attention again. Owners can copy their booking link and preview the customer journey.

Customers choose a service, specialist and appointment time, then manage their own reservations. Staff see their assigned appointments and time off. Managers organize service categories, staff skills, schedules and scoped account access. Working time includes service duration and preparation buffers; rescheduling checks availability again.

Shared Persian date, time and searchable selection controls work across salon and platform forms. They support keyboard operation and local digits while preserving the booking time contract. The interface uses Persian typography, right-to-left layouts, light/dark themes and reduced-motion behavior. The catalogue includes dimensional beauty artwork with a static fallback.

## Growth — customer relationships and loyalty

The same customer record connects appointments, service-specific CRM history and follow-ups. A manager assigned to selected service lines sees only the authorized service context; common customer identity does not expose unrelated service notes.

Marketing creates internal CRM work for service recalls, inactive customers, first-visit follow-up, loyal visitors and missed appointments. Campaigns can run once or weekly. Consent exclusions, existing appointments, open follow-ups and cooldowns affect eligibility. Campaigns organize team work; they do not send promotional SMS or Push. Subsequent bookings are a correlation, not proven campaign revenue.

The salon club awards points for eligible completed services and net collections after discounts/refunds. Managers configure general or service-specific rules, availability delays, expiry, recognition levels and non-cash gifts. Customers see their points and redeem gifts; managers record fulfillment. Refunds reconcile earned points, including deficits after prior redemption. Points are not money, and a gift does not automatically reserve an appointment or discount a bill. Birthday/referral campaigns are not connected in this release.

## Intelligence — recorded performance and accounting

Managers can record bills, discounts, manual collections/refunds, staff commissions and settlements. Commission follows net collected amounts for completed services; original rule snapshots preserve past calculations. Repeated submissions do not duplicate financial records, and over-collection/refund limits are enforced.

Operational accounting adds paid expenses and retained corrections, cash movement, receivables, specialist/service performance and a daily CSV export. Reports distinguish current balances from period activity. Recorded cash movement is not bank-confirmed balance, profit, statutory accounting or automated payroll. The product does not move funds or verify an online gateway payment.

## Branches, access and platform administration

Owners can invite existing salons into an organization. Each branch owner approves and controls the permissions, and can change or revoke them. Branches retain their own customers, appointments and financial records; switching workspaces does not merge customer databases or confer platform authority.

A separate platform workspace manages salon directories, plan drafts and subscription lifecycle records. Salon accounts cannot promote themselves to platform operators. Subscription snapshots retain their terms and history. These administrative records do not charge a card or automatically enforce feature limits or expiry lockout.

## Notifications and web app

Beauty includes an in-app inbox, browser Push configuration and installation guidance for the web app. Push requires user permission and browser/device support. Calendar-file downloads are manual imports, not ongoing calendar synchronization.

Kavenegar template settings are available, but real SMS delivery and OTP login remain disconnected. Online payment transport is also disconnected. Verified delivery-based or assisted recovery, platform MFA and broader commercial entitlement enforcement remain future work.

## Release validation

The release passed 243 Beauty tests, six shared Core tests, 11 contract tests and build. Sixty focused catalogue browser states covered four viewport widths in both themes, reversible scroll progression, keyboard anchors, persistent and system reduced motion, unavailable graphics, blocked storage, short landscape, login links and back navigation. Six graphics scenarios checked idle/offscreen rendering and cleanup. The catalogue/role suite passed 147 states, and service-worker replacement preserved an unsaved draft.

After activation, the same 60 catalogue states passed over public HTTPS. All 41 public assets matched the release package. Verification used only public pages: no demo workspace, login session, customer record, financial event or external message was created.

These checks do not establish physical iOS/Android Push receipt, device GPU performance or owner/pilot acceptance. No real purchase, customer financial event or external message was used for presentation testing.

This repository contains public product notes only. Private application source, infrastructure details, credentials and customer data are not published here. Validation describes observed behavior, not a guarantee of availability, security or marketing results.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
