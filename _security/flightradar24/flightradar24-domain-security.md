---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flightradar24.com
  spf: true
hosts:
- cert_expires: Aug 19 17:57:32 2026 GMT
  host: fr24api.flightradar24.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flightradar24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flightradar24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flightradar24
provider_slug: flightradar24
slug: flightradar24-domain-security
source_filename: flightradar24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fr24api.flightradar24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:57:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flightradar24.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/security/flightradar24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aviation
- Flight Tracking
- Real-Time
- Aircraft
- Airports
- Airlines
- ADS-B
- Historical Data
---
