---
api_specs:
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Payouts API
  slug: chimoney-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Wallets API
  slug: chimoney-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Multicurrency Wallets API
  slug: chimoney-multicurrency-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Sub-Accounts API
  slug: chimoney-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Redeem API
  slug: chimoney-redeem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Info API
  slug: chimoney-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Accounts API
  slug: chimoney-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Payments API
  slug: chimoney-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chimoney.io
  spf: false
hosts:
- cert_expires: Oct  2 18:31:45 2026 GMT
  host: chimoney.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 00:21:04 2026 GMT
  host: api.chimoney.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 10:44:51 2026 GMT
  host: api-v2-sandbox.chimoney.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chimoney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chimoney, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Chimoney
provider_slug: chimoney
slug: chimoney-domain-security
source_filename: chimoney-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chimoney.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:31:45 2026 GMT\n  hsts: false\n- host: api.chimoney.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 00:21:04 2026 GMT\n  hsts: false\n- host: api-v2-sandbox.chimoney.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:44:51 2026 GMT\n  hsts: false\ndomains:\n- domain: chimoney.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/security/chimoney-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payouts
- Disbursements
- Payments
- Africa
- Global Payouts
- Wallets
- Multicurrency
- Gift Cards
- Mobile Money
- Fintech
---
