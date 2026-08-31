---
api_specs:
- filename: leanlaw-client-api-openapi.yml
  format: yaml
  label: LeanLaw Client API
  slug: leanlaw-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-client-api-openapi.yml
- filename: leanlaw-codes-api-openapi.yml
  format: yaml
  label: LeanLaw Codes API
  slug: leanlaw-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-codes-api-openapi.yml
- filename: leanlaw-customfield-api-openapi.yml
  format: yaml
  label: LeanLaw Custom Field API
  slug: leanlaw-customfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-customfield-api-openapi.yml
- filename: leanlaw-expense-api-openapi.yml
  format: yaml
  label: LeanLaw Expense API
  slug: leanlaw-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-expense-api-openapi.yml
- filename: leanlaw-fixedfee-api-openapi.yml
  format: yaml
  label: LeanLaw Fixed Fee API
  slug: leanlaw-fixedfee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-fixedfee-api-openapi.yml
- filename: leanlaw-invoice-api-openapi.yml
  format: yaml
  label: LeanLaw Invoice API
  slug: leanlaw-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-invoice-api-openapi.yml
- filename: leanlaw-matter-api-openapi.yml
  format: yaml
  label: LeanLaw Matter API
  slug: leanlaw-matter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-matter-api-openapi.yml
- filename: leanlaw-practicearea-api-openapi.yml
  format: yaml
  label: LeanLaw Practice Area API
  slug: leanlaw-practicearea-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-practicearea-api-openapi.yml
- filename: leanlaw-timeentry-api-openapi.yml
  format: yaml
  label: LeanLaw Time Entry API
  slug: leanlaw-timeentry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-timeentry-api-openapi.yml
- filename: leanlaw-user-api-openapi.yml
  format: yaml
  label: LeanLaw User API
  slug: leanlaw-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leanlaw.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leanlaw.io
  spf: true
hosts:
- cert_expires: Sep 29 20:33:33 2026 GMT
  host: www.leanlaw.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 11:03:37 2026 GMT
  host: platform.leanlaw.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 13:23:00 2026 GMT
  host: api.leanlaw.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leanlaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeanLaw, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LeanLaw
provider_slug: leanlaw
slug: leanlaw-domain-security
source_filename: leanlaw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leanlaw.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:33:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.leanlaw.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 11:03:37 2026 GMT\n  hsts: false\n- host: api.leanlaw.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 13:23:00 2026 GMT\n  hsts: null\ndomains:\n- domain: leanlaw.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: leanlaw.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/security/leanlaw-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Legal Billing
- Law Firms
- Time Tracking
- Billing
- Invoicing
- Accounting
- Trust Accounting
- Practice Management
- QuickBooks
- Payments
- LegalTech
- SaaS
---
