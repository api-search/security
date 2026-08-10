---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flixbus.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: global.flixbus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: developer.api.flixbus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: global.api.flixbus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flixbus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlixBus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FlixBus
provider_slug: flixbus
slug: flixbus-domain-security
source_filename: flixbus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: global.flixbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: developer.api.flixbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\n- host: global.api.flixbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: flixbus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flixbus/refs/heads/main/security/flixbus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Transportation
- Travel
- Mobility
- Bus
- Rail
- Ticketing
- GTFS
- Open Data
- Distribution
---
