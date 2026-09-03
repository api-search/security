---
certifications: []
description: ''
kind: trust-center
layout: security
name: Formboost Trust Center
name_suffix: Trust Center
overview: Formboost maintains a public trust center covering its security and compliance posture.
provider_name: Formboost
provider_slug: formboost
slug: formboost-trust-center
source_filename: formboost-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://formboost.app/security\nurl: https://formboost.app/security\ntrust_center_published: true\ntrust_center_note: >-\n  Formboost has no separate trust.* subdomain or certification portal. It publishes a single\n  security-and-data-protection page that does the job of one: what is stored, who processes it,\n  how it is protected, retention, GDPR rights, and how to report a vulnerability.\ncertifications: []\ncertifications_note: >-\n  ZERO third-party certifications, stated by the provider in its own words:\n  \"We hold no third-party certifications — no SOC 2 report, no ISO 27001, no independent\n  penetration test to share yet. Anyone claiming otherwise about us is wrong.\"\n  It goes further: \"If your organisation requires a certified processor today, we are not the\n  right fit yet, and we would rather say so than lose your trust later.\"\ncorrection_note: >-\n  CORRECTED 2026-09-02. An earlier automated pass (probe-security-programs.py)\
  \ keyword-matched\n  the strings \"SOC 2\" and \"ISO 27001\" on this page and recorded both as certifications HELD.\n  The page says the exact opposite — the keywords appear inside an explicit disclaimer. The\n  false entries were removed by hand. This is a negation false-positive in the probe script, not\n  a provider claim, and no Compliance pointer is emitted for SOC 2 or ISO 27001.\ncompliance_programs:\n  - name: GDPR\n    status: self-declared\n    detail: >-\n      Genuinely documented rather than merely asserted. The page sets out the controller/processor\n      split (customer is controller of submissions, Formboost is processor), names the data\n      subjects, enumerates every subprocessor with what it can see, describes how to exercise\n      access/portability/erasure, and offers a data processing agreement on request.\n    dpa_available: true\n    dpa_route: email request\n    source: https://formboost.app/security\ndata_handling:\n  sells_data: false\n  sells_data_statement:\
  \ >-\n    \"Submissions are not sold, rented, brokered, or used for advertising or profiling. Formboost\n    makes money from subscriptions, not from your data.\"\n  stored:\n    - category: Submission content\n      detail: Whatever fields the form posts, stored as JSON exactly as submitted.\n    - category: Submission metadata\n      detail: Timestamp, spam score, read state, and the form it belongs to.\n    - category: Account data\n      detail: Email address, and a bcrypt-hashed password or a Firebase identity.\n    - category: Integration config\n      detail: Destination URLs and any custom headers, used to deliver submissions.\n    - category: Billing records\n      detail: Subscription and payment references. Card details are handled by Razorpay only.\n  tracking_on_customer_forms: false\n  tracking_note: >-\n    \"We do not run trackers or fingerprinting on the forms you host.\"\nsubprocessors:\n  published: true\n  commitment: >-\n    \"We do not add a subprocessor that touches\
  \ submission content without updating this list.\"\n  list:\n    - name: Google (Gemini API)\n      purpose: Spam screening\n      sees: Submission content, on plans with AI screening active\n    - name: Google (Firebase)\n      purpose: Sign-in\n      sees: Account email and authentication identifiers\n    - name: Razorpay\n      purpose: Payments and subscriptions\n      sees: Billing identifiers and payment details entered with them\n    - name: Email delivery provider\n      purpose: Notification emails\n      sees: Recipient address and submission contents in the notification\n      note: Not named on the page.\n    - name: Tawk.to\n      purpose: Support chat on formboost.app\n      sees: Chat contents, only after optional cookies are accepted\n    - name: Google Analytics\n      purpose: Website analytics\n      sees: Usage data on formboost.app only — never submission data, and only after consent\ncontrols:\n  transport: TLS on every endpoint, terminated at the edge; Helmet security\
  \ headers on API responses.\n  transport_verified: >-\n    TLSv1.3, HSTS max-age=15552000 includeSubDomains preload, restrictive CSP — probed 2026-09-02.\n  authentication: Signed JWTs for dashboard access; email verification required before the API accepts requests.\n  endpoint_hardening: Per-IP rate limiting, oversized-body rejection, spam screening before storage.\n  webhook_ssrf_control: >-\n    Destinations must be public HTTPS URLs; private and loopback addresses are rejected,\n    \"which prevents Formboost being used to reach internal networks.\"\nretention:\n  automatic_expiry: false\n  detail: >-\n    \"Submissions are kept until you delete them. There is no automatic expiry today, so data\n    minimisation is in your hands.\" Formboost explicitly declines to imply a retention schedule\n    it does not enforce; scheduled retention is on the roadmap.\n  customer_controls:\n    - Export any form's submissions as CSV\n    - Delete individual submissions\n    - Delete a form (deletes\
  \ its submissions)\n    - Delete the account (removes everything)\n  source: https://formboost.app/security\nassessment: >-\n  A young product with no audited assurance, but with unusually honest disclosure. There is no\n  certification to point a procurement team at; there IS a complete, specific and self-critical\n  account of what happens to the data. Buyers requiring a certified processor should read the\n  provider's own advice and look elsewhere for now.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formboost/refs/heads/main/security/formboost-trust-center.yml
summary_line: trust center published
tags:
- forms
- form-backend
- html-forms
- serverless
- static-sites
- react
- nextjs
- vue
- webhooks
- no-code
- developer-tools
- spam-filtering
trust_url: https://formboost.app/security
---
