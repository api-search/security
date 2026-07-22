---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amadeus-hospitality.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: travelclick.com
  spf: true
hosts:
- cert_expires: Sep 15 11:06:02 2026 GMT
  host: www.amadeus-hospitality.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 21:19:37 2026 GMT
  host: developer.travelclick.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelclick Amadeus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TravelClick (Amadeus), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TravelClick (Amadeus)
provider_slug: travelclick-amadeus
slug: travelclick-amadeus-domain-security
source_filename: travelclick-amadeus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amadeus-hospitality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:06:02 2026 GMT\n  hsts: false\n- host: developer.travelclick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:19:37 2026 GMT\n  hsts: null\ndomains:\n- domain: amadeus-hospitality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: travelclick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelclick-amadeus/refs/heads/main/security/travelclick-amadeus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Apps
- Hospitality
- Hotels
- Travel
- Booking Engine
- Reservations
- Distribution
- Central Reservation System
- OAuth2
---
