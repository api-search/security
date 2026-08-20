---
api_specs:
- filename: form3-payments.yml
  format: yaml
  label: Form3 Public API
  slug: form3-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Payments API
  slug: form3-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Direct Debits & Mandates API
  slug: form3-direct-debits-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Account Identification & Verification API
  slug: form3-account-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Files API
  slug: form3-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Event Notifications API
  slug: form3-event-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Security & Access API
  slug: form3-security-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: form3.tech
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.form3.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.api-docs.form3.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.form3.tech
  https: false
kind: domain-security
layout: security
method: probed
name: Form3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Form3, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Form3
provider_slug: form3
slug: form3-domain-security
source_filename: form3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.form3.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.api-docs.form3.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.form3.tech\n  https: false\ndomains:\n- domain: form3.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/security/form3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Payment Processing
- Account-to-Account
- Real-Time Payments
- Faster Payments
- Bacs
- SEPA
- Direct Debit
- Confirmation of Payee
- Cross-Border
- Banking as a Service
- Embedded Payments
---
