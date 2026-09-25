---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: makemytrip.com
  spf: true
hosts:
- cert_expires: Nov  1 05:30:58 2026 GMT
  host: makemytrip.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Makemytrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MakeMyTrip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MakeMyTrip
provider_slug: makemytrip
slug: makemytrip-domain-security
source_filename: makemytrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makemytrip.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 05:30:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: makemytrip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makemytrip/refs/heads/main/security/makemytrip-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Travel
- Booking
- India
---
