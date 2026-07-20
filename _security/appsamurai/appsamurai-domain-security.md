---
api_specs:
- filename: appsamurai-campaign-spend-openapi.yml
  format: yaml
  label: AppSamurai Campaign Spend API
  slug: appsamurai-campaign-spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-campaign-spend-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appsamurai.com
  spf: true
hosts:
- cert_expires: Oct 15 15:04:59 2026 GMT
  host: appsamurai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: help.appsamurai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.appsamurai.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Appsamurai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appsamurai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appsamurai
provider_slug: appsamurai
slug: appsamurai-domain-security
source_filename: appsamurai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appsamurai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:04:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.appsamurai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\n- host: api.appsamurai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: appsamurai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/security/appsamurai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile
- Advertising
- User Acquisition
- Marketing
- App Growth
- Attribution
- Analytics
- Mobile Marketing
- SDK
---
