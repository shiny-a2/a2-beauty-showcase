# A2 Beauty

[Open the product catalogue](https://beauty.amiraliyaghouti.com) · [Sign in](https://beauty.amiraliyaghouti.com/login) · [Request a consultation](https://beauty.amiraliyaghouti.com/start)

Release **0.41.0** connects customer booking, specialist schedules, reception, salon management, specialist rental accounting and a limited AI secretary for demo customers and the demo salon manager in independent salon workspaces. Beauty uses the shared A2 CRM and loyalty engines for customer relationships and service points.

## Lighter startup and a familiar loading scene — 0.41.0

The salon and platform interfaces now load bundled application code and styles. The catalogue's measured JavaScript requests drop from 22 to 3, and stylesheet requests from 7 to 1. Compressed main JavaScript is about 20% smaller, excluding the unchanged 3D scene. These are resource measurements, not a promise of identical speed on every connection or phone.

While information loads, the catalogue's vanity table gently gathers its accessories into place in a short loop. It uses lightweight vector artwork and CSS motion rather than a second 3D engine. Reduced motion keeps the table still, hidden tabs pause the animation, and ready content appears without waiting for the loop to finish. A failed startup stops the movement and offers a clear retry. The initial status paints before application evaluation and decorative WebGL work.

The build and all 395 Beauty checks passed. Local browser verification covered 302 loading, scroll, login, role and operator states in light/dark themes at desktop/mobile widths. Timing samples showed improved median readiness but variable cold-process results; physical-phone performance still needs device testing.

After publication, 99 public loading and scroll states passed over HTTPS, and all 55 served assets matched the release. Slow and failed requests were simulated only in the test browser; no live accounts, leads, bookings or payments were created.

## Persian package names — 0.40.1

The catalogue now uses **پایه** for daily salon work, **رشد** for customer relationships and **هوشمند** for reporting and activation-scoped AI. The same names appear in chapter navigation, consultation choices and the team’s request list. Navigation follows Persian reading direction. Saved requests and existing links stay compatible; package scope, activation requirements and pricing are unchanged.

The patch passed the build, four focused asset/worker checks, 36 local presentation states and 60 existing scroll/motion states. Checks covered light/dark themes, desktop/mobile widths, keyboard navigation and open/selected package choices. Operator request labels used browser-only sample records. Database behavior was unchanged and its migration test was not run for this copy update.

After publication, 36 focused browser states also passed over HTTPS and all 48 served assets matched the release. No live leads, accounts, bookings or payments were created for these checks.

## A clearer first look at the salon experience

The catalogue now offers an interactive preview of four roles: salon management, reception, specialists and customers. Clearly marked example agendas and handoffs explain how the product fits each person's day. Keyboard navigation and reduced motion are supported; the preview does not create accounts, appointments or payments.

The sign-in page brings the salon identity into a sculpted arch and layered beauty tools, with a compact mobile layout. The original scroll-driven vanity remains, alongside clearer feature sections and a direct link to explore the role preview. SMS, payment and AI activation boundaries remain explicit.

Public files now use negotiated compression and browser revalidation; account APIs remain uncached. Seven measured response bodies total 920,269 uncompressed bytes versus 234,751 Brotli bytes, a 74.5% reduction against uncompressed delivery. This measures file bytes, not page-load time or real-phone performance; the 3D scene already supported gzip in earlier releases.

Build, 393 Beauty tests, 21 shared Core tests and 11 contract checks passed. The local matrix passed 295 browser states, including the new preview/login at four widths in both themes, scroll and fallback graphics, keyboard/reduced motion, normal login, isolated demos and existing panels. Physical-device graphics performance and owner design acceptance remain separate.

After publication, all 47 served assets matched and 80 public studio/login states plus 60 scroll/graphics states passed over HTTPS. Live Brotli delivery, conditional 304 responses and the uncached session boundary were verified. The checked text/background token pairs exceed 4.5:1 in both themes. Public checks created no account, demo, appointment, payment or message.

## Book a service again from appointment history

Customers and authorized reception or management staff can start a fresh booking from a completed, cancelled or missed appointment. The current service price and duration are shown, the available original specialist is selected and the customer chooses a new time before confirming. The booking summary now includes service duration.

If a service is unavailable, the page explains how to select another. If the previous specialist no longer offers it, choosing a replacement is explicit. Current access and appointment ownership are checked again, and the original appointment remains unchanged.

Build, 391 Beauty tests, 21 shared Core tests and 11 contract checks passed. Across light/dark mobile and desktop layouts, 76 local rebooking states and 80 booking/search regression states passed. Twelve new appointments were created through the local UI and API with current-price, duration and source-record checks. These used synthetic local data.

After publication, 48 live interface states passed for customers, managers and receptionists in both themes and widths. History/detail reads used browser-only synthetic fixtures; sessions, catalogue and availability came from the live service. All 45 served assets matched. End-to-end booking creation was verified locally, not on production; the live empty test salon was deactivated with no appointments, financial records or outbound messages.

## Find the right service more easily

Booking now includes instant Persian search across service names, descriptions and categories. Common Arabic/Persian spelling and digit variants work together, and the current category keeps the results relevant. Clear result counts and an empty-state message help customers find their way back.

Searching keeps the chosen service, specialist and time. If a selected service falls outside the results, a notice explains that the choice is still in the appointment summary. The search stays inside the browser and does not send the typed words to the server. Existing appointments keep their original service when changing the time.

Build, 387 Beauty tests, 21 shared CRM tests and 11 contract checks passed. Forty-four local search states and 36 calendar/booking states passed across light/dark themes at mobile and desktop widths, including keyboard use, empty results, preserved selections, rescheduling and cancelled-slot availability. Actual booking creation in these checks used local synthetic data.

After publication, 32 live interactive states passed in customer and manager panels across both themes and widths. All 44 served assets matched the release. The synthetic workspace was deactivated and its sessions removed; live checks created no appointments, financial records or external messages.

## Edit services without overwriting a colleague's changes

Service editing now checks the definition and assigned specialists together before saving. If another manager has changed the service, the form keeps the current draft and offers an explicit reload. A changed price, duration or specialist assignment does not rewrite existing appointment snapshots.

Retrying an unchanged save after a lost reply does not create another service or repeat its audit event. If the draft changes while the previous result is uncertain, staff can check that earlier save first and then continue editing the confirmed service. The saved form stays open until its list refreshes, so immediately reopening it shows the saved values. A failed refresh also retains the confirmed service identity.

The implementation passed 382 Beauty tests, 21 shared CRM tests and 11 contract checks. The final interface patch passed 30 focused regression checks, 56 service-editor browser states and the existing 112-state colleague onboarding and booking-to-refund journey. Browser checks covered both themes and mobile/desktop widths, with synthetic local data and no external messages. The quick-reopen fix followed a failure found during the first live check; that failed result is not counted as a successful release check.

The published 0.37.1 release passed 20 live browser states with four synthetic service-description saves and immediate rereads. All 43 served assets matched. Both test workspaces were deactivated and their sessions removed; live checks created no appointment, financial record or external message.

## Follow up after a completed service

Managers can set an optional aftercare delay for each service and use it in an internal CRM campaign. The campaign considers the customer's latest completed visit to the selected service, starting at its configured due time and continuing for seven days. Existing opt-outs, marketing exclusions, future bookings, open follow-ups and contact cooldowns still apply. The same visit cannot generate another aftercare task through a different campaign.

Aftercare starts disabled for existing services, and saving a delay does not activate a campaign. Staff explicitly create and activate a draft, with source-visit details available in the campaign report. The suggested text asks the team to review the salon's approved instructions and the customer's experience; it does not generate treatment advice or send advertisements. Service-setting conflicts offer an explicit reload, and the form reuses the Persian calendar and custom dropdowns.

Build, 373 Beauty tests, 21 shared CRM tests and 11 contract checks passed. The local browser matrix passed 48 interactive states in light/dark themes at mobile and desktop widths. Additional focused checks verified that recorded source visits remain compatible with demo cleanup. Positive aftercare generation, consent exclusions and concurrent execution were tested with local synthetic data.

The published release passed 32 live browser states, including four service-setting saves and four unactivated draft campaigns. All 43 served assets matched the release. Live checks created no appointment, financial record, CRM task or external message; the test workspace was deactivated afterward. Physical-device Push and salon pilot acceptance remain separate checks.

## Give each follow-up a responsible colleague

Authorized CRM staff can assign an open follow-up from its queue card or customer profile. The picker shows the current colleague, searches eligible names and paginates longer teams. The task card then names the responsible colleague. The existing task keeps its subject, due time and campaign links.

Only active colleagues with CRM access to the task's salon and service can receive it. Assignment does not grant new access. Permissions are rechecked when saving, and stale forms cannot overwrite another change or reassign completed work. Lost-reply retries do not duplicate a transfer. The interface reuses the product's custom dropdown with keyboard support.

Build, 365 Beauty tests, 21 shared CRM tests and 11 contract checks passed. The focused browser matrix passed 64 assignment states and 64 existing editing states across light/dark mobile/desktop layouts. It covered search, pagination, empty results, stale selections, revoked recipients, lost replies, retry and dismissed reads.

The published release also passed 24 live browser states with four synthetic transfers reread through the API. All 43 served assets matched the release. Live verification created no booking, financial record or external message.

## Keep an existing follow-up up to date

Reception and authorized CRM staff can change an open follow-up's subject and due time from the work queue or customer profile. The editor uses the Persian calendar and Tehran time. The same task stays linked to its customer and campaign, with its assignee preserved. Saving an unchanged form keeps the original precise due time.

A stale form cannot overwrite another colleague's edit or reopen completed work. The draft stays visible with an explicit reload action, and retrying after a lost reply does not duplicate the update. Existing salon, service and assignment permissions apply; unsupported integrations do not gain this capability automatically.

Build, 356 Beauty tests, 18 shared CRM tests and 11 contract checks passed. The browser checks covered 64 editing states and 60 work-queue regression states in light/dark themes at mobile/desktop widths, including the Persian date picker, stale drafts, lost replies, read retries and long text.

The published release passed 24 additional live browser states and four synthetic task edits reread through the API. All 43 served assets matched the release. Live QA created no booking, financial record or external message.

## See the periods behind fixed rent

Managers and specialists with access to their own statements can inspect the exact periods behind the fixed-rent total. Each row shows its start/end dates, governing contract start and fixed amount. More than twenty periods can be browsed, and a collapsible section keeps long statements manageable. Failed reads offer a retry for the same account and page; late responses cannot replace a dismissed or newer view.

The total and its detail rows use the same calculation. Existing balances, payment records, service commissions and future contract start dates are preserved. Dates display in Persian; existing rental periods still follow their recorded Gregorian month boundaries. A future calendar conversion and first-month proration need a separate policy and compatible transition. Period rows explain a balance and are not payment receipts.

Build, 350 Beauty tests, 15 shared CRM tests, 11 contract checks and 96 local interactive browser states passed. The local tests cover positive rent, more than twenty months, leap/year boundaries, agreement changes, exact rial totals and denied cross-account/salon access. Light/dark and mobile/desktop layouts, disclosure keyboard use, retry and dismissed responses were checked. The final patch removes an obsolete footer version label; ten focused checks and the 56 period/statement browser states passed again.

The published release passed 32 additional read-only browser states across authorized manager and specialist views, and all 43 served assets matched the release. Empty test workspaces were deactivated after verification. Positive rent and long histories were tested locally; live checks created no booking, financial record or external message.

## Correct contact details while retaining consent history

Reception and authorized CRM staff can correct a supplemental contact with recorded consent, explain why it changed and review the information before and after the correction. The history identifies the person who recorded the change and its time. Salon, service-line and private-contact access apply to both current details and historical entries.

A changed phone or email does not inherit positive marketing consent: the current status becomes unknown. An existing opt-out remains in effect. Name-only corrections preserve the status, and edits to a linked customer's account phone follow the same rule. Marketing uses current consent, not old entries in the history. Repeated saves with the same receipt do not duplicate a correction.

Validation passed 344 Beauty tests, 15 shared CRM tests, 11 contract checks and 96 local interactive browser states in light/dark mobile/desktop layouts. Checks included stale edits, lost-response retries, authorization changes, transactional failure recovery, history pagination and the marketing consumer. The final patch also ties health reporting to the packaged release version, with a regression for health/cache consistency. Historical edits are not backfilled; automatic customer merging and physical-device Push acceptance remain separate work.

Live verification passed 16 interactive states and four synthetic contact corrections. All 43 served assets matched the release package. The test workspace was deactivated and its sessions removed; no live appointment, financial record or external message was created by these checks.

## Different hours for each weekday

Managers with team access can give a specialist different hours on different days, add up to four shifts in a day, close a day or end work at midnight. For example, a morning shift and an afternoon shift leave a real gap in the booking calendar. The existing Persian clock controls are used throughout.

Availability, new bookings, rescheduling and the demo secretary use the same booking calculation. A service and its preparation time must fit inside a working interval; existing reservations prevent an incompatible schedule change. Setup guidance checks the individual intervals rather than the total span of the day. Previous schedules keep their behavior until edited, and recorded appointment times and financial calculations are preserved.

The editor retains drafts when another manager changes the schedule, offers a deliberate reload and retries an unchanged save once without repeating its effect. It reads back the saved schedule before closing, so reopening immediately shows the latest intervals. Validation covered the build, 333 Beauty tests, 11 shared CRM tests, 11 contract checks and 200 local interactive browser states across daily editing, Persian booking calendars and colleague setup. Mobile/desktop and light/dark layouts were inspected.

After the final activation, 16 live interactive states and four synthetic schedule saves passed without page errors or horizontal overflow. The booking API offered no times in the split-shift gap or closed day, and all 43 public assets matched the release package. Test workspaces were deactivated. No live appointment, financial record or external message was created by these checks. Physical-device Push and broader commercial/pilot acceptance remain separate work.

## Review customer records that share a phone

Reception and authorized CRM staff can find other accessible records with the same phone, open a related profile and return to the same result page. Iranian mobile prefixes and Persian/Arabic digits are recognized through the shared CRM engine. Salon, service-line and private-contact permissions constrain both the source and results.

A shared phone can belong to family members; this review does not establish identity or merge customer records. Existing contact correction and consent protections remain. Loading, empty results, retry and dismissed requests have explicit behavior.

The combined release preserves 0.30.6's demo secretary improvements. Build, 322 Beauty tests, 11 shared CRM tests and 11 contract checks passed. Local browser validation covered 56 shared-phone states, 52 contact-correction regression states and four inherited photo-review views across mobile/desktop and light/dark themes. After activation, 20 live interactive states passed without page errors or horizontal overflow, and 42 public assets matched the release package. The synthetic demo was deactivated; no appointment, financial record or external message was created by these live checks. Automatic merging remains future work; consent-history correction is included in 0.32.1 above.

## Safer service and appointment guidance in the demo

When a customer names several different services, the AI secretary no longer offers times for an arbitrary one. It checks availability across more eligible specialists, orders the suggested times and asks the customer to confirm the final choice in the normal booking flow. Answers based on an uploaded photo now visibly explain that a salon specialist must review the image before a final decision. This update does not add a staff review queue.

The limited demo AI budget and access scope are unchanged. The shared manager agent for CRM reports and approved follow-ups remains a separate preview. The Beauty build and all 314 local tests passed; the photo notice was inspected in light and dark at mobile and desktop widths. After activation, 42 public assets matched the release package and four public page states opened without page errors or horizontal overflow. The live authenticated photo conversation was not exercised during this release check.

## Correct a customer contact without changing their account

Beauty 0.30.5 lets authorized CRM and reception staff correct supplemental contact names, phone numbers and email addresses through the shared A2 CRM engine. Separate cards distinguish account-owned details, additional contacts and private information. The existing account editor remains available only to staff with the corresponding permission; contacts with recorded consent remain protected from this correction form.

Stale edits keep the draft and offer an explicit refresh. Retrying after a lost response records the correction once, and closing a dialog prevents a delayed save from reopening it. Corrections retain their salon and service scope, with an audit entry. Duplicate contact merging and consent-history correction remain separate planned work.

The build, 313 Beauty tests, nine shared CRM tests and 11 contract tests passed. Fifty-two local browser states covered manager/reception flows, identity synchronization, stale edits, connection loss, long values and dismissal in both themes at mobile/desktop widths. After release, 12 live interactive states and four synthetic contact corrections passed, and 42 served assets matched the package. No appointment, financial record or external message was created by these live checks. Independent applications keep their current CRM package until separately upgraded.

## From a new colleague to a reconciled balance

Beauty 0.30.4 guides managers from colleague creation through service assignment, working hours, the applicable commission or rental agreement and booking preview. Selecting percentage-only rental terms now shows only the salon percentage; fixed rent and service commission keep their own relevant fields and explanations. Current and scheduled contracts show separate effective dates, and specialist contract reads require the appropriate permission.

Commission drafts stay with their original colleague and service when switching selections. Stale changes offer a refresh, dismissed dialogs stay closed after delayed responses, and rent receipt history continues beyond the first page. The update reuses the shared booking, CRM and finance paths without changing recorded balances or recurring-rent calculations. Dates display in Persian; existing rental billing periods still follow their established calendar pending a separate migration.

The build, 306 Beauty tests, six Core tests and 11 contract tests passed. Local browser acceptance covered 264 interactive mobile/desktop light/dark states, including new-colleague booking, discounted billing, partial collection, payout, refund adjustment and the linked CRM record. After publication, 36 interactive live manager states passed without page errors or horizontal overflow, and 42 served assets matched the release. Financial journeys used synthetic local data; live checks created no appointment, financial transaction or external message. Physical-device and pilot acceptance remain separate.

## Shared manager agent preview

A disabled source candidate connects salon manager text chat to the same assistant core as Education. It can read authorized CRM reports and propose internal follow-ups; creating or completing a task requires the manager's explicit confirmation. The existing photo, catalog and booking assistant remains available on its current path.

The candidate passed 31 focused Beauty regression tests, 15 shared integration checks with scripted model output and combined mobile/desktop light/dark interface checks. It has not been deployed; production access/runtime activation, durable chat and scheduled reporting remain pending. See the [shared platform engineering note](https://github.com/shiny-a2/a2-intelligence-showcase).

## Find the assistant from the catalogue

The product catalogue now links directly to the demo sign-in from a small animated assistant card. It explains that `visitor12` can enter without a password. The هوشمند chapter, role descriptions and FAQ distinguish the service and appointment guidance available in the manager and customer demos from AI features that still need separate activation. The assistant suggests candidate times; booking confirmation stays in the regular flow.

Beauty 0.30.3 passed its build and all 300 automated checks. Local browser checks covered 155 catalogue and demo states, and 60 motion states including reduced motion and narrow screens. After publication, four light/dark mobile/desktop catalogue states passed interaction and layout checks, and the public catalogue assets matched the release package.

## An assistant that stays with the demo manager

The demo salon manager now sees a small animated mirror control on every workspace screen. It opens the AI assistant for questions about current services and candidate appointment times. Text works without a photo; an optional photo needs explicit consent. The assistant cannot read balances, sales or customer records, and it never confirms a booking. The existing overall demo spend cap and per-user quota also apply to manager conversations. AI remains disabled for managers of non-demo salons.

Beauty 0.30.2 passed its build and all 300 automated checks. The scoped AI bridge passed its build and 14 focused checks. A live synthetic demo manager received a text-only AI response; four mobile/desktop light/dark states showed the launcher and opened conversation without page errors or horizontal overflow. Keyboard focus and reduced-motion behavior were checked. The test demo was deactivated, and the AI usage receipt settled below both demo caps. No appointment or salon financial record was created for this check.

## Specialist contracts and balances

Release 0.30.0 lets salon managers choose a specialist's commission, fixed monthly desk rent, fixed rent plus the salon's percentage of net collected completed services, or percentage-only terms. Specialist statements and accounting views show rent received and the resulting balance for both sides. Terms, receipts and financial history remain scoped to each salon.

The Persian AI secretary is now live for signed-in **demo customers**. It offers service guidance and available appointment suggestions, accepts an optional photo with explicit consent, and hands the customer to the normal booking flow for confirmation. It does not reserve an appointment on its own. The demo service has an overall spend cap and a separate quota for each customer. Activation for non-demo salons remains a separate decision.

The 0.30.1 release passed the Beauty build and 300 automated checks, including consent, photo submission, account separation and rental calculations. The separate AI bridge passed its build and 14 focused checks. A live synthetic demo customer sent one test message with a generated image and received an AI reply; the receipt stayed within both spend caps. Four live interactive desktop and mobile theme states passed without page errors or horizontal overflow. The test demo was then deactivated.

For the earlier 0.30.0 accounting release, thirty-six local interactive mobile and desktop states passed in light and dark themes, including chat, photo, booking handoff, contract and balance views. After deployment, all 200 package files and 44 public HTTPS assets matched that release. Twelve fully rendered public browser states passed in both themes at mobile and desktop widths, without page errors or horizontal overflow. Existing records and access restrictions were checked for preservation during the schema upgrade. Those checks used synthetic local finance data and public-only live browsing; authenticated live rent remains unverified. No live financial record or external message was created for presentation tests.

## A vanity that becomes organized as you scroll

Release 0.29.0 replaces the small mirror display with a full vanity desk and fifteen salon tools. Scrolling lifts the scattered brushes, bottles, makeup and accessories, aligns them in the air and places them neatly on the desk. Reversing the scroll retraces the same paths; brushes arrive after their holder.

The desk stays grounded, and mobile gives the scene more room. Reduced motion shows the arranged desk immediately; devices without WebGL receive a matching static illustration. Rendering settles when input stops and pauses when the scene is offscreen. The existing chapter links, keyboard navigation, themes, login and consultation links remain available.

Build, five focused automated checks and sixty local catalogue browser states passed. The separate scene harness checked forward/reverse poses, theme changes, pointer settling, cleanup/remount and graphics fallback. Validation used headless Chrome with software WebGL, not physical-device GPU benchmarks. Version 0.29.0 was the previous live release. All sixty interactive catalogue states passed again over HTTPS after its deployment, with no page errors or horizontal overflow. All 43 public assets matched that release package. Verification used public pages only, with no accounts, demo salons, financial records or external messages created.

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

The catalogue now describes SMS, online payments and AI capabilities as separately activated offerings. Proposed هوشمند capabilities include campaign copy assistance, customer visit-pattern analysis and management summaries. These require implementation/activation; they do not run in the current demo. Scope, activation conditions and pricing are agreed before a contract.

## A catalogue that follows your scroll

Version 0.24 keeps a three-dimensional beauty studio beside the product story. Scrolling through the introduction, پایه, رشد and هوشمند changes the studio angle, accessory positions and artwork while the feature text stays readable. Scrolling back restores earlier poses. Chapter links support the keyboard and show the current section.

The studio adapts to mobile, desktop and short landscape layouts. A Reduce motion control remembers the visitor's choice, and the device's reduced-motion setting takes precedence. If browser graphics are unavailable, an illustrated fallback remains. Rendering settles when input stops and pauses while the scene is out of view. Native scrolling, login links and the existing theme control remain available.

## Explore the product

The catalogue presents three groups of capabilities: **پایه**, **رشد** and **هوشمند**. Final package composition and pricing are agreed during consultation. Features marked as requiring activation are not represented as live demo functionality.

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

## پایه — daily salon work

Platform operators create salon accounts after coordination. Owners then follow setup tasks for specialists, services and prices, working hours and the salon address. Progress reflects current configuration: deactivating a specialist can make a service need attention again. Owners can copy their booking link and preview the customer journey.

Customers choose a service, specialist and appointment time, then manage their own reservations. Staff see their assigned appointments and time off. Managers organize service categories, staff skills, schedules and scoped account access. Working time includes service duration and preparation buffers; rescheduling checks availability again.

Shared Persian date, time and searchable selection controls work across salon and platform forms. They support keyboard operation and local digits while preserving the booking time contract. The interface uses Persian typography, right-to-left layouts, light/dark themes and reduced-motion behavior. The catalogue includes dimensional beauty artwork with a static fallback.

## رشد — customer relationships and loyalty

The same customer record connects appointments, service-specific CRM history and follow-ups. A manager assigned to selected service lines sees only the authorized service context; common customer identity does not expose unrelated service notes.

Marketing creates internal CRM work for service recalls, inactive customers, first-visit follow-up, loyal visitors and missed appointments. Campaigns can run once or weekly. Consent exclusions, existing appointments, open follow-ups and cooldowns affect eligibility. Campaigns organize team work; they do not send promotional SMS or Push. Subsequent bookings are a correlation, not proven campaign revenue.

The salon club awards points for eligible completed services and net collections after discounts/refunds. Managers configure general or service-specific rules, availability delays, expiry, recognition levels and non-cash gifts. Customers see their points and redeem gifts; managers record fulfillment. Refunds reconcile earned points, including deficits after prior redemption. Points are not money, and a gift does not automatically reserve an appointment or discount a bill. Birthday/referral campaigns are not connected in this release.

## هوشمند — reporting and activation-scoped AI

Proposed AI assistance covers campaign drafts, customer visit-pattern analysis and management summaries, with human review. These capabilities need separate implementation and activation. The current demo includes the limited service-and-appointment assistant described above; it does not provide these proposed CRM or reporting capabilities.

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
