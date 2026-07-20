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
- cert_expires: Mar 15 19:05:22 2027 GMT
  host: api-docs.hoteltonight.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 15 19:05:22 2027 GMT
  host: api.hoteltonight.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hoteltonight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HotelTonight, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HotelTonight
provider_slug: hoteltonight
slug: hoteltonight-domain-security
source_filename: hoteltonight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hoteltonight.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 15 19:05:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.hoteltonight.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 15 19:05:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hoteltonight.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 15 19:05:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hoteltonight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hoteltonight/refs/heads/main/security/hoteltonight-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Travel
- Hotels
- Booking
- Hospitality
- Partner API
- Airbnb
---
