---
api_specs:
- filename: shiftmove-fleet-openapi.json
  format: json
  label: Avrios Fleet-API
  slug: avrios-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-fleet-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avrios.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.avrios.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shiftmove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shiftmove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shiftmove
provider_slug: shiftmove
slug: shiftmove-domain-security
source_filename: shiftmove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.avrios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: avrios.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/security/shiftmove-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fleet Management
- Mobility
- Automotive
- Telematics
- Vehicles
- Fleet API
- SaaS
---
