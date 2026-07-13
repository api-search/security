---
api_specs:
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Core Accounting API
  slug: campfire-hq-core-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Chart of Accounts & Company Objects API
  slug: campfire-hq-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Financial Statements API
  slug: campfire-hq-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Accounts Payable API
  slug: campfire-hq-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Accounts Receivable API
  slug: campfire-hq-accounts-receivable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Revenue Recognition API
  slug: campfire-hq-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Cash Management API
  slug: campfire-hq-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Bank Reconciliation API
  slug: campfire-hq-bank-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Settings API
  slug: campfire-hq-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Integrations & Webhooks API
  slug: campfire-hq-integrations-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: campfire.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: meetcampfire.com
  spf: true
hosts:
- cert_expires: Sep 14 23:22:18 2026 GMT
  host: www.campfire.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 19:13:37 2026 GMT
  host: docs.campfire.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: api.meetcampfire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Campfire Hq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campfire, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Campfire
provider_slug: campfire-hq
slug: campfire-hq-domain-security
source_filename: campfire-hq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.campfire.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:22:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.campfire.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:13:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.meetcampfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: campfire.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: meetcampfire.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/security/campfire-hq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- ERP
- General Ledger
- Revenue Recognition
- FinTech
- AI
---
