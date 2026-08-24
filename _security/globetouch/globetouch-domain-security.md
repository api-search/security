---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airlinq.com
  spf: true
hosts:
- cert_expires: Oct 15 00:09:02 2026 GMT
  host: www.airlinq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Globetouch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globetouch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Globetouch
provider_slug: globetouch
slug: globetouch-domain-security
source_filename: globetouch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airlinq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 00:09:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airlinq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globetouch/refs/heads/main/security/globetouch-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- IoT
- Connectivity
- eSIM
- SIM Management
- Telecommunications
- Mobile
- Connected Vehicles
- Utilities
- Roaming
---
