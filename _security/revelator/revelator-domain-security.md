---
api_specs:
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Distribution API
  slug: revelator-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Catalog API
  slug: revelator-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Analytics API
  slug: revelator-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Royalties & Accounting API
  slug: revelator-royalties-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Payments & Wallet API
  slug: revelator-payments-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revelator.com
  spf: true
hosts:
- cert_expires: Sep 22 08:51:23 2026 GMT
  host: www.revelator.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 01:58:03 2026 GMT
  host: api-docs.revelator.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  3 19:19:45 2027 GMT
  host: api.revelator.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revelator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revelator, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revelator
provider_slug: revelator
slug: revelator-domain-security
source_filename: revelator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revelator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:51:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.revelator.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 14 01:58:03 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.revelator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 19:19:45 2027 GMT\n  hsts: false\ndomains:\n- domain: revelator.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/security/revelator-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Distribution
- Rights
- Royalties
- Payments
- Analytics
---
