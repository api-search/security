---
api_specs:
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Transactions API
  slug: tithely-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Payments & Tokenization API
  slug: tithely-payments-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Organizations API
  slug: tithely-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Payment Categories (Funds) API
  slug: tithely-payment-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Mail API
  slug: tithely-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Accounts API
  slug: tithely-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tithe.ly
  spf: true
hosts:
- cert_expires: Oct  2 01:11:29 2026 GMT
  host: get.tithe.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: tithe.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 05:41:00 2026 GMT
  host: docs.tithe.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tithely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tithe.ly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tithe.ly
provider_slug: tithely
slug: tithely-domain-security
source_filename: tithely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: get.tithe.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tithe.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tithe.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:41:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tithe.ly\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/security/tithely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Church Giving
- Donations
- Fundraising
- Payments
- Nonprofit
- ChMS
- Faith
---
