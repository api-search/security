---
api_specs:
- filename: llms.txt
  format: yaml
  label: Truckstop Load Management API
  slug: truckstop-load-management-api
  spec_type: OpenAPI
  url: https://developer.truckstop.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: truckstop.com
  spf: true
hosts:
- cert_expires: Dec 12 17:13:59 2026 GMT
  host: truckstop.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 12:36:25 2026 GMT
  host: developer.truckstop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:09:22 2026 GMT
  host: api.truckstop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truckstop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truckstop, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Truckstop
provider_slug: truckstop
slug: truckstop-domain-security
source_filename: truckstop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truckstop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 17:13:59 2026 GMT\n  hsts: false\n- host: developer.truckstop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.truckstop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:09:22 2026 GMT\n  hsts: null\ndomains:\n- domain: truckstop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truckstop/refs/heads/main/security/truckstop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Load Board
- Trucking
- Logistics
- Freight Marketplace
- Carrier Search
- Rate Insights
- Transportation
- Broker
- Shipper
---
