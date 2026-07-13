---
api_specs:
- filename: pleo-bookkeeping-core-openapi.yml
  format: yaml
  label: Pleo Bookkeeping Core API
  slug: pleo-bookkeeping-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-bookkeeping-core-openapi.yml
- filename: pleo-gjoll-openapi.yml
  format: yaml
  label: Pleo Gjoll API
  slug: pleo-gjoll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-gjoll-openapi.yml
- filename: pleo-triton-openapi.yml
  format: yaml
  label: Pleo Triton API
  slug: pleo-triton-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-triton-openapi.yml
- filename: pleo-oberon-openapi.yml
  format: yaml
  label: Pleo Oberon API
  slug: pleo-oberon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-oberon-openapi.yml
- filename: pleo-export-openapi.yml
  format: yaml
  label: Pleo Export API
  slug: pleo-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-export-openapi.yml
- filename: pleo-tax-code-openapi.yml
  format: yaml
  label: Pleo Tax Code API
  slug: pleo-tax-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-tax-code-openapi.yml
- filename: pleo-tags-openapi.yml
  format: yaml
  label: Pleo Tags API
  slug: pleo-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-tags-openapi.yml
- filename: pleo-app-marketplace-openapi.yml
  format: yaml
  label: Pleo App Marketplace API
  slug: pleo-app-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-app-marketplace-openapi.yml
- filename: pleo-vendors-openapi.yml
  format: yaml
  label: Pleo Vendors API
  slug: pleo-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-vendors-openapi.yml
- filename: pleo-webhook-subscriptions-openapi.yml
  format: yaml
  label: Pleo Webhook Subscriptions API
  slug: pleo-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-webhook-subscriptions-openapi.yml
- filename: pleo-chart-of-accounts-openapi.yml
  format: yaml
  label: Pleo Chart of Accounts API
  slug: pleo-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/openapi/pleo-chart-of-accounts-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pleo.io
  spf: true
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: www.pleo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 16:19:05 2026 GMT
  host: developers.pleo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:27:23 2026 GMT
  host: external.pleo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pleo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pleo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pleo
provider_slug: pleo
slug: pleo-domain-security
source_filename: pleo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pleo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.pleo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 16:19:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: external.pleo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:27:23 2026 GMT\n  hsts: null\ndomains:\n- domain: pleo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pleo/refs/heads/main/security/pleo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Expense Management
- Company Cards
- Spend Management
- Reimbursements
- Accounting
- FinTech
- Finance
---
