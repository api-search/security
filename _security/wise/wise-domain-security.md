---
api_specs:
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Profiles API
  slug: profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Recipients API
  slug: recipients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Transfers API
  slug: transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Balances API
  slug: balances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Multi-Currency Account API
  slug: multi-currency-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Statements API
  slug: statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Simulation API
  slug: simulation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wise.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: wise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: docs.wise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.wise.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wise, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wise
provider_slug: wise
slug: wise-domain-security
source_filename: wise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.wise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/security/wise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- FX
- Cross-Border
- Banking
- Multi-Currency
---
