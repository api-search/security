---
api_specs:
- filename: virtual-peaker-gravity-connect-device-partner-api-openapi.yml
  format: yaml
  label: Gravity Connect API (Device Partner)
  slug: gravity-connect-device-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml
- filename: virtual-peaker-gravity-connect-vpp-api-openapi.yml
  format: yaml
  label: Gravity Connect API (Virtual Peaker)
  slug: gravity-connect-vpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-gravity-connect-vpp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: virtual-peaker.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: virtualpeaker.io
  spf: true
hosts:
- cert_expires: Oct  1 19:00:47 2026 GMT
  host: virtual-peaker.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: assets.virtualpeaker.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: partner.virtualpeaker.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virtual Peaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtual Peaker, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Virtual Peaker
provider_slug: virtual-peaker
slug: virtual-peaker-domain-security
source_filename: virtual-peaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virtual-peaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 19:00:47 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: assets.virtualpeaker.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\n- host: partner.virtualpeaker.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: virtual-peaker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: virtualpeaker.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/security/virtual-peaker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Grid
- Demand Response
- DER
- DERMS
- Virtual Power Plant
- EV Charging
- Smart Thermostats
- Energy Storage
---
