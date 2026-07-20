---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hoteltonight.com
  spf: true
hosts:
- cert_expires: Mar 15 19:05:22 2027 GMT
  host: www.hoteltonight.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hotel Tonight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hotel Tonight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hotel Tonight
provider_slug: hotel-tonight
slug: hotel-tonight-domain-security
source_filename: hotel-tonight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hoteltonight.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 15 19:05:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hoteltonight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotel-tonight/refs/heads/main/security/hotel-tonight-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Travel
- Hotels
- Booking
- Hospitality
- Mobile
- Airbnb
---
