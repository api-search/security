---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flightnetwork.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tripstack.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.flightnetwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: ca.flightnetwork.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 13:14:21 2026 GMT
  host: www.tripstack.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flight Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flight Network, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flight Network
provider_slug: flight-network
slug: flight-network-domain-security
source_filename: flight-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flightnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\n- host: ca.flightnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: www.tripstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:14:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: flightnetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tripstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flight-network/refs/heads/main/security/flight-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Canada
- Aviation
- Airline
- OTA
- Booking
- Distribution
- Flights
- Hotels
- Car Rental
- GDS
---
