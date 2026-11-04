# A2 Beauty

[Open the product catalogue](https://beauty.amiraliyaghouti.com) · [Sign in](https://beauty.amiraliyaghouti.com/login) · [Request a consultation](https://beauty.amiraliyaghouti.com/start)

Release **0.29.0** connects customer booking, specialist schedules, reception and salon management in independent salon workspaces. Beauty uses the shared A2 CRM and loyalty engines for customer relationships and service points.

## A vanity that becomes organized as you scroll

Release 0.29.0 replaces the small mirror display with a full vanity desk and fifteen salon tools. Scrolling lifts the scattered brushes, bottles, makeup and accessories, aligns them in the air and places them neatly on the desk. Reversing the scroll retraces the same paths; brushes arrive after their holder.

The desk stays grounded, and mobile gives the scene more room. Reduced motion shows the arranged desk immediately; devices without WebGL receive a matching static illustration. Rendering settles when input stops and pauses when the scene is offscreen. The existing chapter links, keyboard navigation, themes, login and consultation links remain available.

Build, five focused automated checks and sixty local catalogue browser states passed. The separate scene harness checked forward/reverse poses, theme changes, pointer settling, cleanup/remount and graphics fallback. Validation used headless Chrome with software WebGL, not physical-device GPU benchmarks. Version 0.29.0 is live. All sixty interactive catalogue states passed again over HTTPS after deployment, with no page errors or horizontal overflow. All 43 public assets matched the release package. Verification used public pages only, with no accounts, demo salons, financial records or external messages created.

## Clearer panels for daily salon work

Release 0.28.0 uses warmer Persian instructions and separates appointment time, service, people, status and actions into readable cards. Appointments are grouped by Tehran date; each group count refers to the current page. Quick period filters remain visible, with extra filters available on demand.

CRM customer cards open the full file with a click or Enter. Follow-ups distinguish upcoming, overdue and completed work. Team schedules, reception shortcuts, services and notification context have clearer visual separation, using the existing Beauty illustrations and shared light/dark theme. Booking behavior and role permissions are retained.

Build, 18 focused automated tests and 348 local browser states passed. The browser suites cover panel interactions, booking calendars, CRM work queues, notifications and custom date/dropdown controls, including keyboard use, long names, small screens and both themes. Version 0.28.0 was deployed before the current vanity-scene update. After deployment, 56 interactive HTTPS states passed on mobile/desktop in light/dark themes, including booking, rescheduling, cancellation, filter submission, customer files and reception. All 43 public assets matched the release package. No real customer messages or financial transactions were created.

## Booking dates and working hours

Release 0.27.2 fixes editing working hours that end at midnight: managers can explicitly select the end of the day, while normal closing times retain exact minutes. Calendar month navigation preserves keyboard focus. A booking page re-rendered after Tehran midnight advances an expired day selection and clears its old time.

All 47 focused automated checks passed, covering Persian date conversion and leap boundaries, past times and the five-minute lead boundary, working days, leave, preparation buffers, concurrent reservations, customer/provider overlap, rescheduling and cancellation. Thirty-six local interactive states passed on mobile/desktop in light/dark themes, with device zones set to Los Angeles and Tokyo. Browser/API journeys preserved Tehran booking times, rejected slots extending beyond closing, and released capacity after cancellation. Delayed availability responses preserved the latest selected day. No real customer messages or financial records were created. Version 0.27.2 was deployed before the current panel refresh. Thirty-two interactive HTTPS states passed after deployment, including saved midnight hours and actual booking, rescheduling, cancellation and restored availability in an isolated demo. All 43 public assets matched the release package.

## Install Beauty on your device

Release 0.27.1 adds a compact install invitation inside the manager, reception, specialist and customer panels. Supported browsers offer installation after a click; iPhone and Android users can open device-specific home-screen guidance. Later hides the invitation for seven days in that browser. It stays hidden when Beauty is already running as an installed app, and it preserves work in progress.

The invitation uses the existing appearance and theme controls. Installing does not grant notification permission automatically, and current salon information and booking still require internet access.

The build, 13 focused regression checks and 75 local browser checks passed. Browser install events and device user agents were simulated; physical-device installation remains unverified. At the 0.27.1 deployment, 48 interactive HTTPS states passed across all four roles, both themes and mobile/desktop with no page errors or horizontal overflow. All 43 public assets matched the release package. No real customer messages or financial transactions were created.

## Notification center

Release 0.27.0 adds an unread bell and a shared notification center for salon managers, reception, specialists and customers. Filters separate unread messages, appointment reminders, attendance and booking changes. Cards show the current service, time and status, with relevant customer/specialist context and direct appointment details. Authorized staff can confirm completion or no-show through the existing booking workflow.

Day-before and one-hour reminders use the existing delivery worker. An overdue appointment prompts authorized staff to check attendance; it never automatically marks a customer absent. The customer is notified of no-show only after a permitted staff member records it. Repeated processing does not duplicate the same reminder stage, and cancelled, rescheduled, reassigned or no-longer-authorized delivery is suppressed. Historical reminder wording clearly distinguishes an old message from the current appointment state.

Local validation covered 294 distinct Beauty checks and 96 interactive browser states across four roles, mobile/desktop and light/dark themes. Build and shared-module checks passed. No real customer messages or financial transactions were used. At the 0.27.0 deployment, 96 interactive HTTPS states passed across four roles, both themes and mobile/desktop. The live worker generated both reminder stages in isolated demos; filters, appointment details, reading state and unread badges worked without page errors or horizontal overflow. All 42 public assets matched the release package. Test salons were deactivated after verification. Real-device Push receipt and SMS activation remain pending.

## Reception, CRM and cashier access

Reception staff now have their own workspace. A salon owner creates a reception account and selects booking, customer relationship and cashier access individually. A new account starts without work permissions and must change its initial password. The same person can handle all three areas or only the assigned work.

Cashier permissions distinguish viewing bills, issuing bills and recording collections, discounts/quoted prices, refunds and voiding an unpaid bill. Cashier access does not expose commission rules or open accounting, staff settlement, user administration or salon settings. Permission changes close existing sessions. Linking a service to a CRM record now explicitly checks CRM permission, including for delegated accounts. Existing financial records, refund limits, CRM follow-ups and customer loyalty remain on their shared processing paths.

The reception home shows permitted work areas. Mobile navigation keeps reception, appointments, customers and cashier directly accessible when assigned, with other permitted destinations in the menu. The demo offers reception as a fourth workspace.

A shared product-protection roadmap also covers commercial licensing, copyright notices, abuse controls and release protection across A2 products. It is planned work; this release does not activate commercial license enforcement. Backend source remains private, while code delivered to a browser is inherently inspectable.

## Shared licensing groundwork

The shared licensing source now supports an optional signed product association, so a Beauty observer can distinguish its own product license from an unrelated one. Legacy clients keep their existing validation behavior. Product-aware checks reject wrong products, missing required claims and downgrade to an older unbound response.

The monitor remains passive: it does not grant user permissions or lock salon accounts. A separate operator tool reports verified policy evidence while retaining safe failure behavior. A packaging correction also makes the authority schema definitions available in a fresh source checkout.

Local validation passed 19 license tests, including both PHP authority contracts and the actual Beauty operator tool, plus the workspace build, six Core tests and 11 contract tests. Seven authority PHP suites and the existing admin browser regression passed, including mobile/desktop light/dark layouts. Product, HTTP and WordPress compatibility checks also passed from a clean source archive. All data was synthetic; no live authority or customer records were used.

The shared licensing groundwork is packaged with Beauty 0.27.0, but central product/salon provisioning, commercial limits and live authority integration remain pending. The monitor is not activated and existing salon access is unchanged.

## Independent salon licenses and usage reports

The commercial model now specifies one independent license per salon. New private operator tooling reads one salon's aggregate account usage without changing its data or access. It separates active team accounts, inactive accounts, customers, branch delegates and system accounts. Owners are included once in the team total. Linked salons retain their own license scope.

An explicitly selected reporting policy can supply these aggregate counts to a product-aware license refresh. Separate private caches reject accidental reuse across salons or authority mappings. The report does not include customer names, contact details or financial records. These counts describe accounts; commercial seat limits still require agreement.

Local validation passed 273 Beauty tests, including eight new usage checks, 19 shared license tests, six Core tests, 11 contract tests and build, with no skips. Tests used synthetic PostgreSQL records and covered salon isolation, concurrent changes, enforced read-only transactions, cache separation and the actual operator tool. Refresh integration used a synthetic signed response; no live authority connection is claimed.

The private tooling is packaged with 0.27.0 and is not exposed in salon panels. No live usage refresh is activated and license enforcement stays inactive.

## Audited salon license assignments

New private tooling registers each salon's association with a central license and installation. Database constraints prevent either active identifier from being assigned to two salons in the same Beauty database. Registration checks a recent signed product policy, and only privileged maintenance operations attributed to an active platform operator can change an association.

Expected revisions reject stale changes, exact retries do not duplicate records, and assignment/history/audit updates commit together. Local revocation blocks the next mapped refresh without deleting history or revoking the central license. Usage reports show whether an association is unassigned, matched, mismatched or revoked. An already approved passive request may finish; this is not user-access enforcement.

Local validation passed 284 Beauty tests, 19 shared license tests, six Core tests, 11 contract tests and build, with no skips. Coverage includes competing salon registrations, duplicate identifiers, denied permissions, rollback on audit/history failure, the private command and repeatable migration preserving existing accounts. Demo cleanup also protects salons with assignment history. All records were synthetic.

The additive local registry structures are included in the 0.27.0 update, with access restricted to private maintenance tooling. No real salon has been assigned through this work, no central license was issued or changed, and commercial access remains unchanged.

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

## Earlier reception validation

Local validation covered 265 distinct Beauty tests across the full suite and focused reception/migration runs, six shared Core tests, 11 contract tests and build. Checks included independent permissions, initial-password onboarding, cross-salon denial, CRM commands, cashier restrictions, retries/refund limits, queued-access revocation, booking notifications, migration replay and recovery compatibility.

Sixty-two reception browser states and 147 catalogue/login/existing-role states passed across light/dark desktop and mobile layouts, with no page errors or horizontal overflow. Interactive checks included account creation and editing, focus, separate modules, a synthetic collection confirmation, read-only cashier access, mobile menus and demo switching. Service-worker replacement preserved an unsaved draft. All financial and account records used for these checks were synthetic and local.

After the earlier 0.26.0 activation, all 41 public assets matched the release package and 36 public HTTPS browser states passed in both themes at desktop/mobile widths, without page errors or horizontal overflow. Seven private/source paths denied access and four protected APIs required authentication. Public checks made no API writes. That earlier public-only check did not cover authenticated workflows. The 0.27.0 notification journey described above adds authenticated demo verification; external payment/message delivery remains unverified.

These checks do not establish physical iOS/Android Push receipt, device GPU performance or owner/pilot acceptance. No real purchase, customer financial event or external message was used for presentation testing.

This repository contains public product notes only. Private application source, infrastructure details, credentials and customer data are not published here. Validation describes observed behavior, not a guarantee of availability, security or marketing results.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
