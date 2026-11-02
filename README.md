# A2 Beauty

A salon needs one appointment workflow that customers, specialists and managers can all trust. A2 Beauty brings these three views together: customers choose a service and available specialist, specialists manage their schedule, and managers maintain the service catalog and customer follow-ups.

The first release supports independent salon workspaces, nested service categories, configurable appointment lengths and prices, staff availability, cancellation and rescheduling. Booking connects to the shared A2 CRM domain so customer relationships and follow-ups continue after an appointment is made.

The interface is Persian and right-to-left, with Jalali dates, light and dark themes, responsive layouts and an installable web-app shell. A clearly marked demonstration creates a separate synthetic salon where visitors can switch among the three roles.

## Validation

Six shared Core tests and fifteen application integration scenarios passed, including tenant separation, role restrictions, concurrent booking conflicts, retry safety and transaction rollback. Ten browser journeys passed across four desktop/mobile and light/dark combinations. A backup restored into a separate disposable database matched nineteen tables. These checks establish the tested scope, not a guarantee of availability or security.

## Release scope

Version 0.1.0 provides the initial booking and CRM workflow. Online payment, SMS delivery, subscription billing, commission settlement and multi-branch chains are not enabled. This repository contains public product notes only; application source, deployment configuration and customer data remain private.

Built by [Amir Ali Yaghouti](https://amiraliyaghouti.com) as part of A2.
