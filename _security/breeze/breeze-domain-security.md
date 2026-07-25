---
api_specs:
- filename: breeze-admin-api-openapi.yml
  format: yaml
  label: Breeze Admin API
  slug: breeze-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-admin-api-openapi.yml
- filename: breeze-deposits-api-openapi.yml
  format: yaml
  label: Breeze Deposits API
  slug: breeze-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-deposits-api-openapi.yml
- filename: breeze-fund-api-openapi.yml
  format: yaml
  label: Breeze fund API
  slug: breeze-fund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-fund-api-openapi.yml
- filename: breeze-funds-api-openapi.yml
  format: yaml
  label: Breeze Funds API
  slug: breeze-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-funds-api-openapi.yml
- filename: breeze-global-config-api-openapi.yml
  format: yaml
  label: Breeze Global Config API
  slug: breeze-global-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-global-config-api-openapi.yml
- filename: breeze-organization-api-keys-api-openapi.yml
  format: yaml
  label: Breeze Organization API Keys API
  slug: breeze-organization-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-organization-api-keys-api-openapi.yml
- filename: breeze-organization-api-openapi.yml
  format: yaml
  label: Breeze Organization API
  slug: breeze-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-organization-api-openapi.yml
- filename: breeze-organization-funds-api-openapi.yml
  format: yaml
  label: Breeze Organization Funds API
  slug: breeze-organization-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-organization-funds-api-openapi.yml
- filename: breeze-organization-settings-api-openapi.yml
  format: yaml
  label: Breeze Organization Settings API
  slug: breeze-organization-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-organization-settings-api-openapi.yml
- filename: breeze-selective-yield-sources-api-openapi.yml
  format: yaml
  label: Breeze Selective Yield Sources API
  slug: breeze-selective-yield-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-selective-yield-sources-api-openapi.yml
- filename: breeze-strategies-api-openapi.yml
  format: yaml
  label: Breeze Strategies API
  slug: breeze-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-strategies-api-openapi.yml
- filename: breeze-strategy-api-openapi.yml
  format: yaml
  label: Breeze Strategy API
  slug: breeze-strategy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-strategy-api-openapi.yml
- filename: breeze-user-data-api-openapi.yml
  format: yaml
  label: Breeze User Data API
  slug: breeze-user-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-user-data-api-openapi.yml
- filename: breeze-withdrawals-api-openapi.yml
  format: yaml
  label: Breeze Withdrawals API
  slug: breeze-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-withdrawals-api-openapi.yml
- filename: breeze-yield-sources-api-openapi.yml
  format: yaml
  label: Breeze Yield Sources API
  slug: breeze-yield-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-yield-sources-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: breeze.com
  spf: true
hosts:
- cert_expires: Sep 11 05:19:22 2026 GMT
  host: breeze.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 07:47:50 2026 GMT
  host: api.breeze.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Breeze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breeze, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Breeze
provider_slug: breeze
slug: breeze-domain-security
source_filename: breeze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breeze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:19:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.breeze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 07:47:50 2026 GMT\n  hsts: null\ndomains:\n- domain: breeze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/security/breeze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Solana
- Yield
- DeFi
- Payments
- Blockchain
- API
- AI Agents
---
