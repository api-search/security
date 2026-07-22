---
api_specs:
- filename: volteras-connect-openapi-original.json
  format: json
  label: Volteras Connect API
  slug: volteras-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volteras/refs/heads/main/openapi/volteras-connect-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: volteras.com
  spf: true
hosts:
- cert_expires: Sep 13 15:34:34 2026 GMT
  host: volteras.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.volteras.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.sandbox.volteras.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Volteras Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volteras, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Volteras
provider_slug: volteras
slug: volteras-domain-security
source_filename: volteras-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volteras.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:34:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.volteras.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\n- host: api.sandbox.volteras.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: volteras.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volteras/refs/heads/main/security/volteras-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electric Vehicles
- Connected Vehicles
- Automotive
- Vehicle Telemetry
- EV Charging
- Energy
- Mobility
- Fleet Management
---
