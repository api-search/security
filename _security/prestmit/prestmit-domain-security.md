---
api_specs:
- filename: prestmit-bank-accounts-api-openapi.yml
  format: yaml
  label: Prestmit Bank Accounts API
  slug: prestmit-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-bank-accounts-api-openapi.yml
- filename: prestmit-general-api-openapi.yml
  format: yaml
  label: Prestmit General API
  slug: prestmit-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-general-api-openapi.yml
- filename: prestmit-gift-cards-buy-api-openapi.yml
  format: yaml
  label: Prestmit Gift Cards - Buy API
  slug: prestmit-gift-cards-buy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-gift-cards-buy-api-openapi.yml
- filename: prestmit-gift-cards-sell-api-openapi.yml
  format: yaml
  label: Prestmit Gift Cards - Sell API
  slug: prestmit-gift-cards-sell-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-gift-cards-sell-api-openapi.yml
- filename: prestmit-lookup-api-openapi.yml
  format: yaml
  label: Prestmit Lookup API
  slug: prestmit-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-lookup-api-openapi.yml
- filename: prestmit-wallet-api-openapi.yml
  format: yaml
  label: Prestmit Wallet API
  slug: prestmit-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-wallet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prestmit.io
  spf: true
hosts:
- cert_expires: Aug 23 05:58:20 2026 GMT
  host: prestmit.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 13:46:15 2026 GMT
  host: api.prestmit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 06:14:01 2026 GMT
  host: dev-api.prestmit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prestmit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prestmit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prestmit
provider_slug: prestmit
slug: prestmit-domain-security
source_filename: prestmit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prestmit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 05:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prestmit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 13:46:15 2026 GMT\n  hsts: false\n- host: dev-api.prestmit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:14:01 2026 GMT\n  hsts: false\ndomains:\n- domain: prestmit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/security/prestmit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bills
- Crypto
- Fintech
- Gift Cards
- Payments
---
