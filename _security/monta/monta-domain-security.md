---
api_specs:
- filename: monta-authentication-api-openapi.yml
  format: yaml
  label: Monta Authentication API
  slug: monta-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-authentication-api-openapi.yml
- filename: monta-charge-points-api-openapi.yml
  format: yaml
  label: Monta Charge Points API
  slug: monta-charge-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-charge-points-api-openapi.yml
- filename: monta-charges-api-openapi.yml
  format: yaml
  label: Monta Charges API
  slug: monta-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-charges-api-openapi.yml
- filename: monta-utilities-api-openapi.yml
  format: yaml
  label: Monta Utilities API
  slug: monta-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-utilities-api-openapi.yml
- filename: monta-wallet-transactions-api-openapi.yml
  format: yaml
  label: Monta Wallet Transactions API
  slug: monta-wallet-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/openapi/monta-wallet-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monta.com
  spf: true
hosts:
- cert_expires: Aug 13 15:20:40 2026 GMT
  host: www.monta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:58:58 2026 GMT
  host: docs.public-api.monta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 14:25:43 2026 GMT
  host: public-api.monta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Monta
provider_slug: monta
slug: monta-domain-security
source_filename: monta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 15:20:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.public-api.monta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:58:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.monta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 14:25:43 2026 GMT\n  hsts: null\ndomains:\n- domain: monta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/security/monta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EV Charging
- Electric Vehicles
- Charge Points
- Energy
- Mobility
---
