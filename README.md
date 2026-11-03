# A2 Beauty

[Open the product catalogue](https://beauty.amiraliyaghouti.com) · [Sign in](https://beauty.amiraliyaghouti.com/login) · [Request a consultation](https://beauty.amiraliyaghouti.com/start)

Release **0.26.0** connects customer booking, specialist schedules, reception and salon management in independent salon workspaces. Beauty uses the shared A2 CRM and loyalty engines for customer relationships and service points.

## Notification center — next-release source

The 0.27.0 source candidate adds an unread bell and a shared notification center for salon managers, reception, specialists and customers. Filters separate unread messages, appointment reminders, attendance and booking changes. Cards show the current service, time and status, with relevant customer/specialist context and direct appointment details. Authorized staff can confirm completion or no-show through the existing booking workflow.

Day-before and one-hour reminders use the existing delivery worker. An overdue appointment prompts authorized staff to check attendance; it never automatically marks a customer absent. The customer is notified of no-show only after a permitted staff member records it. Repeated processing does not duplicate the same reminder stage, and cancelled, rescheduled, reassigned or no-longer-authorized delivery is suppressed. Historical reminder wording clearly distinguishes an old message from the current appointment state.

Local validation covered 294 distinct Beauty checks and 96 interactive browser states across four roles, mobile/desktop and light/dark themes. Build and shared-module checks passed. No real customer messages or financial transactions were used. This is published source preparation, not a live activation: the deployed product remains 0.26.0. Real-device Push verification and SMS activation remain pending.

## Reception, CRM and cashier access

Reception staff now have their own workspace. A salon owner creates a reception account and selects booking, customer relationship and cashier access individually. A new account starts without work permissions and must change its initial password. The same person can handle all three areas or only the assigned work.

Cashier permissions distinguish viewing bills, issuing bills and recording collections, discounts/quoted prices, refunds and voiding an unpaid bill. Cashier access does not expose commission rules or open accounting, staff settlement, user administration or salon settings. Permission changes close existing sessions. Linking a service to a CRM record now explicitly checks CRM permission, including for delegated accounts. Existing financial records, refund limits, CRM follow-ups and customer loyalty remain on their shared processing paths.

The reception home shows permitted work areas. Mobile navigation keeps reception, appointments, customers and cashier directly accessible when assigned, with other permitted destinations in the menu. The demo offers reception as a fourth workspace.

A shared product-protection roadmap also covers commercial licensing, copyright notices, abuse controls and release protection across A2 products. It is planned work; this release does not activate commercial license enforcement. Backend source remains private, while code delivered to a browser is inherently inspectable.

## Shared licensing groundwork

The shared licensing source now supports an optional signed product association, so a Beauty observer can distinguish its own product license from an unrelated one. Legacy clients keep their existing validation behavior. Product-aware checks reject wrong products, missing required claims and downgrade to an older unbound response.

The monitor remains passive: it does not grant user permissions or lock salon accounts. A separate operator tool reports verified policy evidence while retaining safe failure behavior. A packaging correction also makes the authority schema definitions available in a fresh source checkout.

Local validation passed 19 license tests, including both PHP authority contracts and the actual Beauty operator tool, plus the workspace build, six Core tests and 11 contract tests. Seven authority PHP suites and the existing admin browser regression passed, including mobile/desktop light/dark layouts. Product, HTTP and WordPress compatibility checks also passed from a clean source archive. All data was synthetic; no live authority or customer records were used.

These are published source changes, not a production activation. Beauty remains on release 0.26.0. Real product/salon provisioning, commercial limits and live integration remain pending. Existing salon access is unchanged.

## Independent salon licenses and usage reports

The commercial model now specifies one independent license per salon. New private operator tooling reads one salon's aggregate account usage without changing its data or access. It separates active team accounts, inactive accounts, customers, branch delegates and system accounts. Owners are included once in the team total. Linked salons retain their own license scope.

An explicitly selected reporting policy can supply these aggregate counts to a product-aware license refresh. Separate private caches reject accidental reuse across salons or authority mappings. The report does not include customer names, contact details or financial records. These counts describe accounts; commercial seat limits still require agreement.

Local validation passed 273 Beauty tests, including eight new usage checks, 19 shared license tests, six Core tests, 11 contract tests and build, with no skips. Tests used synthetic PostgreSQL records and covered salon isolation, concurrent changes, enforced read-only transactions, cache separation and the actual operator tool. Refresh integration used a synthetic signed response; no live authority connection is claimed.

The source is published; this tooling is not deployed or exposed in the salon panels. Beauty remains on 0.26.0 and license enforcement stays inactive.

## Audited salon license assignments

New private tooling registers each salon's association with a central license and installation. Database constraints prevent either active identifier from being assigned to two salons in the same Beauty database. Registration checks a recent signed product policy, and only privileged maintenance operations attributed to an active platform operator can change an association.

Expected revisions reject stale changes, exact retries do not duplicate records, and assignment/history/audit updates commit together. Local revocation blocks the next mapped refresh without deleting history or revoking the central license. Usage reports show whether an association is unassigned, matched, mismatched or revoked. An already approved passive request may finish; this is not user-access enforcement.

Local validation passed 284 Beauty tests, 19 shared license tests, six Core tests, 11 contract tests and build, with no skips. Coverage includes competing salon registrations, duplicate identifiers, denied permissions, rollback on audit/history failure, the private command and repeatable migration preserving existing accounts. Demo cleanup also protects salons with assignment history. All records were synthetic.

This source candidate requires an additive database migration. It has not been applied to production and no real salon has been assigned through this work. The live Beauty application remains 0.26.0; salon panels and commercial access remain unchanged.

## Tell us about your salon

Version 0.25 replaces public account creation with a consultation request. Visitors choose a package and provide their salon name, contact details, city and requirements, with consent to follow up about that request. Submission returns a reference without creating a salon, login account or customer record.

Platform management opens on a request inbox with new, in-progress and closed states, contact details, follow-up notes and filtering. Operators can create salon accounts after coordination; each owner must change the initial password. Salon accounts cannot read this inbox or create new salon workspaces.

The catalogue now describes SMS, online payments and AI capabilities as separately activated offerings. Proposed Intelligence capabilities include campaign copy assistance, customer visit-pattern analysis and management summaries. These require implementation/activation; they do not run in the current demo. Scope, activation conditions and pricing are agreed before a contract.

## A catalogue that follows your scroll

Version 0.24 keeps a three-dimensional beauty studio beside the product story. Scrolling through the introduction, Essential, Growth and Intelligence changes the studio angle, accessory positions and artwork while the feature text stays readable. Scrolling back restores earlier poses. Chapter links support the keyboard and show the current section.

The studio adapts to mobile, desktop and short landscape layouts. A Reduce motion control remembers the visitor's choice, and the device's reduced-motion setting takes precedence. If browser graphics are unavailable, an illustrated fallback remains. Rendering settles when input stops and pauses while the scene is out of view. Native scrolling, login links and the existing theme control remain available.

## Explore the product

The catalogue presents three groups of capabilities: **Essential**, **Growth** and **Intelligence**. Final package composition and pricing are agreed during consultation. Features marked as requiring activation are not represented as live demo functionality.

Enter **visitor12** on the login page and leave the password empty to open an isolated, populated demo. Switch between manager, reception, specialist and customer panels to explore related services, appointments, CRM records, marketing work, financial reports and loyalty gifts. A connected sample branch demonstrates permission-based access.

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

Platform operators create salon accounts after coordination. Owners then follow setup tasks for specialists, services and prices, working hours and the salon address. Progress reflects current configuration: deactivating a specialist can make a service need attention again. Owners can copy their booking link and preview the customer journey.

Customers choose a service, specialist and appointment time, then manage their own reservations. Staff see their assigned appointments and time off. Managers organize service categories, staff skills, schedules and scoped account access. Working time includes service duration and preparation buffers; rescheduling checks availability again.

Shared Persian date, time and searchable selection controls work across salon and platform forms. They support keyboard operation and local digits while preserving the booking time contract. The interface uses Persian typography, right-to-left layouts, light/dark themes and reduced-motion behavior. The catalogue includes dimensional beauty artwork with a static fallback.

## Growth — customer relationships and loyalty

The same customer record connects appointments, service-specific CRM history and follow-ups. A manager assigned to selected service lines sees only the authorized service context; common customer identity does not expose unrelated service notes.

Marketing creates internal CRM work for service recalls, inactive customers, first-visit follow-up, loyal visitors and missed appointments. Campaigns can run once or weekly. Consent exclusions, existing appointments, open follow-ups and cooldowns affect eligibility. Campaigns organize team work; they do not send promotional SMS or Push. Subsequent bookings are a correlation, not proven campaign revenue.

The salon club awards points for eligible completed services and net collections after discounts/refunds. Managers configure general or service-specific rules, availability delays, expiry, recognition levels and non-cash gifts. Customers see their points and redeem gifts; managers record fulfillment. Refunds reconcile earned points, including deficits after prior redemption. Points are not money, and a gift does not automatically reserve an appointment or discount a bill. Birthday/referral campaigns are not connected in this release.

## Intelligence — reporting and activation-scoped AI

Proposed AI assistance covers campaign drafts, customer visit-pattern analysis and management summaries, with human review. These capabilities need separate implementation and activation; executable AI is not part of the current demo.

Managers can record bills, discounts, manual collections/refunds, staff commissions and settlements. Commission follows net collected amounts for completed services; original rule snapshots preserve past calculations. Repeated submissions do not duplicate financial records, and over-collection/refund limits are enforced.

Operational accounting adds paid expenses and retained corrections, cash movement, receivables, specialist/service performance and a daily CSV export. Reports distinguish current balances from period activity. Recorded cash movement is not bank-confirmed balance, profit, statutory accounting or automated payroll. The product does not move funds or verify an online gateway payment.

## Branches, access and platform administration

Only platform operators can create new branch connections between existing salons. The platform interface begins with appointment-viewing permission; the branch owner can subsequently change or revoke the granted access. Salon sessions cannot create organizations, invite branches or accept connection invitations. Branches retain their own customers, appointments and financial records; switching workspaces does not merge customer databases or confer platform authority.

A separate platform workspace manages sales requests, salon account creation, branch connections, directories, plan drafts and subscription lifecycle records. Salon accounts cannot promote themselves to platform operators. Subscription snapshots retain their terms and history. These administrative records do not charge a card or automatically enforce feature limits or expiry lockout.

## Notifications and web app

Beauty includes an in-app inbox, browser Push configuration and installation guidance for the web app. Push requires user permission and browser/device support. Calendar-file downloads are manual imports, not ongoing calendar synchronization.

Kavenegar template settings are available, but real SMS delivery and OTP login remain disconnected. Online payment transport is also disconnected. Verified delivery-based or assisted recovery, platform MFA and broader commercial entitlement enforcement remain future work.

## Release validation

Local validation covered 265 distinct Beauty tests across the full suite and focused reception/migration runs, six shared Core tests, 11 contract tests and build. Checks included independent permissions, initial-password onboarding, cross-salon denial, CRM commands, cashier restrictions, retries/refund limits, queued-access revocation, booking notifications, migration replay and recovery compatibility.

Sixty-two reception browser states and 147 catalogue/login/existing-role states passed across light/dark desktop and mobile layouts, with no page errors or horizontal overflow. Interactive checks included account creation and editing, focus, separate modules, a synthetic collection confirmation, read-only cashier access, mobile menus and demo switching. Service-worker replacement preserved an unsaved draft. All financial and account records used for these checks were synthetic and local.

After activation, all 41 public assets matched the release package and 36 public HTTPS browser states passed in both themes at desktop/mobile widths, without page errors or horizontal overflow. Seven private/source paths denied access and four protected APIs required authentication. Public checks made no API writes. Live authenticated workflows and external payment/message delivery are not claimed by these checks.

These checks do not establish physical iOS/Android Push receipt, device GPU performance or owner/pilot acceptance. No real purchase, customer financial event or external message was used for presentation testing.

This repository contains public product notes only. Private application source, infrastructure details, credentials and customer data are not published here. Validation describes observed behavior, not a guarantee of availability, security or marketing results.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
