---
api_specs:
- filename: origin-airbrush-openapi-original.yml
  format: yaml
  label: Origin Trades API (Airbrush v3)
  slug: origin-trades-api-airbrush-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin/refs/heads/main/openapi/origin-airbrush-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: originmarkets.com
  spf: true
hosts:
- cert_expires: Aug 27 01:03:19 2026 GMT
  host: originmarkets.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: airbrush.originmarkets.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Origin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Origin, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Origin
provider_slug: origin
slug: origin-domain-security
source_filename: origin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: originmarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 01:03:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: airbrush.originmarkets.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: originmarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origin/refs/heads/main/security/origin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Capital Markets
- Bond Issuance
- Debt Capital Markets
- Fixed Income
- Post-Trade
- ISO 20022
- FinTech
- Straight-Through Processing
---
