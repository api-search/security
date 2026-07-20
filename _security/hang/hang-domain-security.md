---
api_specs:
- filename: hang-partner-api-openapi.yml
  format: yaml
  label: Hang Partner API
  slug: hang-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-partner-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hang.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hang.xyz
  spf: true
hosts:
- cert_expires: Oct 16 19:42:49 2026 GMT
  host: www.hang.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:29:19 2026 GMT
  host: docs.hang.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:33:46 2026 GMT
  host: loyalty.hang.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hang, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hang
provider_slug: hang
slug: hang-domain-security
source_filename: hang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:42:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:29:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: loyalty.hang.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:33:46 2026 GMT\n  hsts: null\ndomains:\n- domain: hang.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hang.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/security/hang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Loyalty
- Rewards
- Membership
- Customer Engagement
- Marketing
- Restaurants
- Point of Sale
- Webhooks
---
