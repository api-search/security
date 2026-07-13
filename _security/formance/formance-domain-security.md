---
api_specs:
- filename: formance-openapi.yml
  format: yaml
  label: Formance Ledger API
  slug: formance-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Payments API
  slug: formance-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Orchestration API
  slug: formance-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Wallets API
  slug: formance-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Reconciliation API
  slug: formance-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Auth API
  slug: formance-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Webhooks API
  slug: formance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
- filename: formance-openapi.yml
  format: yaml
  label: Formance Search API
  slug: formance-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/openapi/formance-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formance.com
  spf: true
hosts:
- cert_expires: Sep 27 15:06:18 2026 GMT
  host: www.formance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:00:48 2026 GMT
  host: docs.formance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Formance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Formance
provider_slug: formance
slug: formance-domain-security
source_filename: formance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.formance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:06:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.formance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:00:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: formance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/security/formance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Infrastructure
- Ledger
- Double-Entry Accounting
- Payments
- Orchestration
- Money Movement
- Open Source
- Fintech
---
