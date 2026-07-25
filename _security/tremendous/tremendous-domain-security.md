---
api_specs:
- filename: tremendous-campaigns-api-openapi.yml
  format: yaml
  label: Tremendous Campaigns API
  slug: tremendous-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-campaigns-api-openapi.yml
- filename: tremendous-funding-sources-api-openapi.yml
  format: yaml
  label: Tremendous Funding Sources API
  slug: tremendous-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-funding-sources-api-openapi.yml
- filename: tremendous-invoices-api-openapi.yml
  format: yaml
  label: Tremendous Invoices API
  slug: tremendous-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-invoices-api-openapi.yml
- filename: tremendous-members-api-openapi.yml
  format: yaml
  label: Tremendous Members API
  slug: tremendous-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-members-api-openapi.yml
- filename: tremendous-orders-api-openapi.yml
  format: yaml
  label: Tremendous Orders API
  slug: tremendous-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-orders-api-openapi.yml
- filename: tremendous-organizations-api-openapi.yml
  format: yaml
  label: Tremendous Organizations API
  slug: tremendous-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-organizations-api-openapi.yml
- filename: tremendous-products-api-openapi.yml
  format: yaml
  label: Tremendous Products API
  slug: tremendous-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-products-api-openapi.yml
- filename: tremendous-rewards-api-openapi.yml
  format: yaml
  label: Tremendous Rewards API
  slug: tremendous-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-rewards-api-openapi.yml
- filename: tremendous-webhooks-api-openapi.yml
  format: yaml
  label: Tremendous Webhooks API
  slug: tremendous-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tremendous.com
  spf: true
hosts:
- cert_expires: Oct  4 04:03:50 2026 GMT
  host: www.tremendous.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 07:19:48 2026 GMT
  host: developers.tremendous.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 04:03:50 2026 GMT
  host: testflight.tremendous.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tremendous Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tremendous, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tremendous
provider_slug: tremendous
slug: tremendous-domain-security
source_filename: tremendous-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tremendous.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:03:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.tremendous.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:19:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: testflight.tremendous.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:03:50 2026 GMT\n  hsts: null\ndomains:\n- domain: tremendous.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/security/tremendous-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Employee Incentives
- Global Payouts
- Incentives
- Market Research
- Payouts
- Rewards
---
