---
api_specs:
- filename: churnkey-billing-contacts-api-openapi.yml
  format: yaml
  label: Churnkey Billing Contacts API
  slug: churnkey-billing-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-billing-contacts-api-openapi.yml
- filename: churnkey-customers-api-openapi.yml
  format: yaml
  label: Churnkey Customers API
  slug: churnkey-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-customers-api-openapi.yml
- filename: churnkey-data-subject-requests-api-openapi.yml
  format: yaml
  label: Churnkey Data Subject Requests API
  slug: churnkey-data-subject-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-data-subject-requests-api-openapi.yml
- filename: churnkey-events-api-openapi.yml
  format: yaml
  label: Churnkey Events API
  slug: churnkey-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-events-api-openapi.yml
- filename: churnkey-sessions-api-openapi.yml
  format: yaml
  label: Churnkey Sessions API
  slug: churnkey-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: churnkey.co
  spf: true
hosts:
- cert_expires: Oct  8 04:48:49 2026 GMT
  host: churnkey.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:15:52 2026 GMT
  host: docs.churnkey.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 01:50:19 2026 GMT
  host: api.churnkey.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Churnkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Churnkey, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Churnkey
provider_slug: churnkey
slug: churnkey-domain-security
source_filename: churnkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: churnkey.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:48:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.churnkey.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:15:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.churnkey.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:50:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: churnkey.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/security/churnkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Churn Prevention
- Retention
- Cancellation Flows
- Failed Payment Recovery
- Dunning
- Reactivation
- Subscriptions
- SaaS
---
