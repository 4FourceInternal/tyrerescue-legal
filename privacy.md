# TyreRescue Privacy Policy

**Last updated: 28 May 2026**

This Privacy Policy explains how the **TyreRescue** mobile application
("the App") collects, uses, stores, shares, and protects information.

The App is operated by **RIB AUTOWORK (PG0544562-V)**, trading as
"Tayar Pancit Ekspres" (the "Operator"). The App is developed and
maintained by **4Fource Technologies** on behalf of the Operator.

By installing or using the App, you agree to the terms of this Privacy
Policy. If you do not agree, please do not install or use the App.

> **Note for end customers:** the TyreRescue mobile App is used only by
> authorised tyre-rescue **workshop staff** and **workshop owners** to
> coordinate roadside rescue jobs. End customers do not use this App —
> customers book a rescue through the website at
> https://tayarpancitekspres.com, which has its own privacy notice. This
> policy therefore covers only data collected from workshop staff and
> owners through the App, and operational data the App displays about
> rescue jobs (including limited customer information needed to perform
> the rescue).

---

## 1. Information we collect

### 1.1 Information you provide directly

When a workshop owner creates a staff account or registers as an owner,
the following information is provided:

- **Identity:** full name, mobile phone number, profile photo (optional,
  uploaded by staff).
- **Business identity** (owners only): business name, business
  registration number, business address.
- **Authentication credentials:** password (stored only as a salted
  Argon2id hash; the cleartext password is never stored or logged).
- **Bank account details** (owners only, for payouts): bank name,
  account number, beneficiary name. Entered through a separate admin
  workflow and stored encrypted at rest.

### 1.2 Information collected automatically while you use the App

- **Precise location (GPS):** when a staff member is actively assigned
  to a rescue job (job status is "EN_ROUTE", "ARRIVED", or
  "IN_PROGRESS"), the App records the staff member's GPS coordinates
  every few seconds and sends them to our servers so that the customer
  can see the staff approaching on their tracking page, and so the
  workshop owner can monitor the staff on the fleet map. **This
  collection includes background location** — i.e. the App continues to
  send GPS while the screen is off, because rescue staff typically have
  the phone mounted on a dashboard or in a pocket while driving.
  Location is **not** collected when no job is active.
- **Device push token:** a Firebase Cloud Messaging (FCM) registration
  token assigned by Google to your installation of the App, used to
  deliver push notifications about new jobs, chat messages, and status
  changes. The token is not personally identifying on its own.
- **Diagnostic data:** when the App crashes or hits an unexpected
  error, an anonymised stack trace and limited contextual data
  (app version, OS version, device model) is sent to our error tracking
  provider (see §3). Personally identifying fields and authentication
  tokens are scrubbed before transmission.

### 1.3 Information the App displays about rescue jobs

When a staff member is assigned a rescue job, the App displays
information about that job, including the customer's first name,
phone number, vehicle details, photo of the damaged tyre, and pickup
location. This information is provided by the customer when they book
the rescue through the website at https://tayarpancitekspres.com. The
mobile App receives this data only to enable the workshop staff to
complete the rescue, and the App does not collect any further data
about the customer beyond what is necessary for the job.

### 1.4 Chat messages

When a workshop owner and a staff member chat about an active job
through the App, the message contents are stored on our servers and
delivered to both participants. Messages are retained for the duration
of the job plus a short audit window (see §5).

### 1.5 What we do **not** collect

- We do not access your photo library except when you explicitly tap
  "Choose photo" to set your staff profile picture.
- We do not access your contacts, calendar, microphone, camera (other
  than the photo-library selector), call log, SMS log, or accounts on
  the device.
- We do not collect advertising identifiers (AAID).
- We do not use the App to collect behavioural-advertising or
  cross-app-tracking data.
- We do not sell any personal information.

---

## 2. Why we collect this information (purpose limitation)

Each category of data has a specific, limited operational purpose:

| Data | Purpose |
| --- | --- |
| Name, phone number, password | Authenticate you when you log in to the App. |
| Profile photo | Display your photo to the customer and your owner so the right staff member can be identified at the rescue site. |
| Business identity | Identify the workshop in dispatch and payment workflows. |
| Bank account (owners) | Process weekly payouts from completed rescue jobs. |
| Precise location (active jobs only) | Show the staff member's live position to the customer on the tracking page, and to the owner on the fleet map. |
| Push token | Deliver notifications about new jobs, chat messages, and status changes. |
| Diagnostic data | Identify and fix bugs and crashes. |
| Chat messages | Allow the owner and staff to coordinate about an active job. |

We do not use any of this information for marketing, behavioural
profiling, or any purpose unrelated to operating the rescue service.

---

## 3. Third-party service providers (data processors)

We use the following third-party service providers to operate the App.
Each acts as a **data processor** — they handle data only on our
instructions and under contract. None receive personal data for their
own marketing or analytics.

| Provider | What they process | Purpose | Provider's privacy notice |
| --- | --- | --- | --- |
| **Google Firebase Cloud Messaging** (Google LLC) | Push registration token, message payloads (no personal content beyond job IDs and brief status text). | Delivering push notifications to your device. | https://firebase.google.com/support/privacy |
| **Cloudinary** (Cloudinary Ltd) | Uploaded photos (staff profile photo, tyre-damage photos). | Image storage and delivery. | https://cloudinary.com/privacy |
| **Sentry** (Functional Software, Inc.) | Anonymised stack traces and crash context. | Error and crash diagnostics. | https://sentry.io/privacy/ |
| **Cloudflare** (Cloudflare, Inc.) | Network-level routing of API traffic between the App and our backend. | Network delivery and DDoS protection. | https://www.cloudflare.com/privacypolicy/ |
| **Mocean SMS** (Micro Ocean Technologies Sdn Bhd) | Phone number, short SMS text. | Fallback SMS notifications if WhatsApp delivery fails. | https://moceanapi.com/privacy-policy/ |
| **Meta WhatsApp Business Platform** (Meta Platforms, Inc.) | Phone number, template message payloads. | Sending booking and status notifications by WhatsApp. | https://www.whatsapp.com/legal/privacy-policy |

Server-side infrastructure (database, file storage, application servers)
is hosted in the Asia-Pacific region by the Maintainer on infrastructure
operated for the App. Specific infrastructure providers may change from
time to time as the service evolves; we will update this Policy when
the change is material (for example, a change in hosting country or
provider).

We do **not** share personal information with advertisers, data brokers,
or any third party not listed above, except where required by law (see
§4).

---

## 4. Legal disclosures

We may disclose personal information if we believe in good faith that
disclosure is required:

- To comply with applicable law, court order, subpoena, or other legal
  process;
- To enforce our terms of service or protect against fraud or abuse;
- To protect the safety, rights, or property of the Operator, our users,
  customers, or the public.

We do not voluntarily provide personal information to law enforcement
without legal process.

---

## 5. Data retention

We retain personal information only as long as needed for the purposes
described in this Policy, or as required by Malaysian law (including
the seven-year record-keeping requirement for commercial transactions
under the Companies Act 2016 and the Income Tax Act 1967, where
applicable).

Specific retention periods:

| Data | Retention |
| --- | --- |
| Account record (name, phone, business info) | While the account is active, and for up to 12 months after deactivation. |
| Authentication credentials (password hash) | Same as account record. Deleted on account deletion. |
| Location history (per-job GPS points) | 30 days after job completion, then deleted. |
| Push registration token | Refreshed by your device automatically; old tokens are purged within 60 days. |
| Job records and chat messages | Up to 7 years for tax and audit purposes (Malaysian statutory record-keeping). |
| Bank payout records (owners) | Up to 7 years for tax and audit purposes. |
| Diagnostic data (Sentry) | 90 days, then automatically purged by Sentry. |

---

## 6. Your rights

Under the Malaysian **Personal Data Protection Act 2010 (PDPA)**, you
have the right to:

- **Access** the personal data we hold about you.
- **Correct** any personal data that is inaccurate, incomplete,
  misleading, or out of date.
- **Withdraw consent** for our processing of your personal data, subject
  to legal and contractual restrictions.
- **Object** to the processing of your personal data for any purpose.
- **Request deletion** of your account and associated personal data
  (see §7 below).
- **Lodge a complaint** with the Personal Data Protection Department
  (Jabatan Perlindungan Data Peribadi), Ministry of Communications.

To exercise any of these rights, contact us using the details in §11.
We will respond within 21 days as required by the PDPA.

---

## 7. Account deletion

You may request deletion of your account and associated personal data
at any time by sending an email to the address in §11.

For us to act on a deletion request, please send the email from an
address you can confirm ownership of, and include the **phone number
registered to your TyreRescue account** in the message body so we can
locate the right record. We may reply with a verification challenge
(for example, sending a short code by SMS to the registered phone
number) before proceeding, to make sure the request comes from the
account holder.

On receipt of a verified deletion request, we will delete your account
record, authentication credentials, profile photo, push registration
token, and location history within 30 days.

The following items **cannot** be deleted on request, because we are
required by Malaysian law (Companies Act 2016, Income Tax Act 1967) to
retain them:

- **Completed-job records** (date, monetary amount, parties involved) —
  retained for up to 7 years after the job, then deleted. We anonymise
  the staff identity in these records on account deletion (replaced
  with "Former staff member" plus an internal ID).
- **Bank payout records** (owners only) — same 7-year retention, same
  anonymisation on account deletion.

Chat messages associated with a deleted account are anonymised within
30 days but the message contents themselves are retained for the same
7-year window for audit and dispute resolution.

If a workshop owner deletes their entire workshop account, all staff
accounts under that workshop are also deleted on the same terms.

---

## 8. Security

We take reasonable steps to protect personal information against
unauthorised access, alteration, disclosure, or destruction:

- All communication between the App and our servers is encrypted in
  transit using TLS 1.2 or higher.
- Passwords are stored only as salted Argon2id hashes; we never store,
  log, or transmit cleartext passwords.
- Bank account details are encrypted at rest in the database.
- Server infrastructure runs in the Asia-Pacific region with
  network-level isolation between application and data tiers.
- Access to production systems is restricted to authorised personnel
  and gated by multi-factor authentication.
- The App's error reporting (Sentry) is configured to scrub
  authentication tokens, password fields, and personally-identifying
  query parameters before transmission.

No system is completely secure. If a data breach occurs and is likely
to result in significant harm, we will notify affected users promptly
and report to the Personal Data Protection Department as required by
Malaysian law.

---

## 9. Children

The App is intended for use by adults working as workshop owners or
staff. The App is not directed at, nor intended for, children under
the age of 13. We do not knowingly collect personal information from
children under 13. If we learn that we have inadvertently collected
such information, we will delete it promptly.

---

## 10. Changes to this Policy

We may update this Privacy Policy from time to time to reflect changes
in our practices or legal requirements. The "Last updated" date at the
top of this document indicates when the policy was last revised.

When we make material changes, we will notify users through the App
(in-app notice) and/or by email or SMS to the registered contact, at
least 14 days before the changes take effect. Continued use of the App
after the effective date constitutes acceptance of the updated Policy.

Prior versions of this Policy are available on request from the
contact in §11.

---

## 11. Contact us

For questions about this Privacy Policy, to exercise your rights under
the PDPA, or to request account deletion, contact us at:

**RIB AUTOWORK (PG0544562-V)**
trading as Tayar Pancit Ekspres
Website: https://tayarpancitekspres.com

**Email:** mohamadsafwan.1905@gmail.com

**Postal address:** [TODO — replace with the Operator's registered business address from the SSM cert before publishing]

Technical support enquiries about the App itself may be directed to the
same email address.

---

## Glossary

- **"App"** — the TyreRescue Android mobile application published on
  Google Play under the package name `com.tyrerescue.app`.
- **"Operator"** — RIB AUTOWORK (PG0544562-V), trading as Tayar Pancit
  Ekspres; the entity that determines the purposes and means of
  processing personal data through the App, and the data controller
  under the PDPA.
- **"Maintainer"** — 4Fource Technologies; the entity that develops and
  operates the App's technical infrastructure on behalf of the
  Operator. Acts as a data processor under the PDPA.
- **"PDPA"** — the Malaysian Personal Data Protection Act 2010.
- **"Workshop staff" / "staff"** — an individual employed or contracted
  by a workshop to perform tyre-rescue jobs, using the App on a mobile
  device.
- **"Workshop owner" / "owner"** — the individual or entity that owns
  or operates a workshop and dispatches staff to perform rescue jobs.
