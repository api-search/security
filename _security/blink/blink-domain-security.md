---
api_specs:
- filename: blink-charging-locations-status-openapi.yml
  format: yaml
  label: Blink Charging Locations & Status API
  slug: blink-charging-locations-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blink/refs/heads/main/openapi/blink-charging-locations-status-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blinkcharging.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: blinknetwork.com
  spf: true
hosts:
- cert_expires: Sep 18 05:04:42 2026 GMT
  host: blinkcharging.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: prod.blinknetwork.com
  https: false
- cert_expires: Feb 13 12:51:03 2027 GMT
  host: api.blinknetwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blink Charging, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blink Charging
provider_slug: blink
slug: blink-domain-security
source_filename: blink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blinkcharging.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 05:04:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod.blinknetwork.com\n  https: false\n- host: api.blinknetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 12:51:03 2027 GMT\n  hsts: null\ndomains:\n- domain: blinkcharging.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: blinknetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blink/refs/heads/main/security/blink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EV Charging
- Electric Vehicle
- Charging Stations
- OCPI
- OCPP
- Fleet Management
- Roaming
- DC Fast Charging
---
