---
api_specs:
- filename: swell-backend-api-openapi.yml
  format: yaml
  label: Swell Backend API
  slug: swell-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/openapi/swell-backend-api-openapi.yml
- filename: swell-frontend-api-openapi.yml
  format: yaml
  label: Swell Frontend API
  slug: swell-frontend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/openapi/swell-frontend-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: swell.is
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swell.store
  spf: true
hosts:
- cert_expires: Aug 31 08:27:44 2026 GMT
  host: www.swell.is
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 15:04:15 2026 GMT
  host: developers.swell.is
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 10:18:16 2026 GMT
  host: api.swell.store
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swell Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swell, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Swell
provider_slug: swell-io
slug: swell-io-domain-security
source_filename: swell-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swell.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:27:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.swell.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:04:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.swell.store\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:18:16 2026 GMT\n  hsts: null\ndomains:\n- domain: swell.is\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: swell.store\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swell-io/refs/heads/main/security/swell-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Headless Commerce
- API-First
- B2C
- B2B
- Subscriptions
- Marketplaces
- Wholesale
- Storefront
- Checkout
- Payments
- Carts
- Orders
- Catalog
- Internationalization
---
