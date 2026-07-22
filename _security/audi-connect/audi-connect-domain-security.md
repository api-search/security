---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audi.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.audi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Audi Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audi Connect / myAudi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Audi Connect / myAudi
provider_slug: audi-connect
slug: audi-connect-domain-security
source_filename: audi-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.audi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: audi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audi-connect/refs/heads/main/security/audi-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Connected Vehicle
- Connected Car
- Telematics
- Mobility
- Remote Control
- Emergency Call
- eCall
- Infotainment
- Electric Vehicle
- EV Charging
- Geofencing
- Stolen Vehicle Recovery
- Fleet
- myAudi
- Audi Connect
- Volkswagen Group
- Germany
---
