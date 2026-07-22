---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toyotaconnected.com
  spf: true
hosts:
- cert_expires: Oct  5 12:23:01 2026 GMT
  host: www.toyotaconnected.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toyota Connected Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toyota Connected, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Toyota Connected
provider_slug: toyota-connected
slug: toyota-connected-domain-security
source_filename: toyota-connected-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.toyotaconnected.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:23:01 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: toyotaconnected.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toyota-connected/refs/heads/main/security/toyota-connected-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Connected Vehicle
- Connected Car
- Telematics
- Mobility
- Mobility Services
- Mobility As A Service
- MSPF
- Drivelink
- Safety Connect
- Service Connect
- Remote Connect
- Destination Assist
- Digital Key
- KINTO
- Car Subscription
- Car Sharing
- Ride Hailing
- Carpooling
- Fleet Telematics
- Big Data
- Voice Assistant
- Toyota
- Lexus
---
