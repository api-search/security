---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tripscout.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: athotel.com
  spf: true
hosts:
- cert_expires: Oct  3 23:56:39 2026 GMT
  host: tripscout.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: athotel.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tripscout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TripScout, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TripScout
provider_slug: tripscout
slug: tripscout-domain-security
source_filename: tripscout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripscout.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:56:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: athotel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: tripscout.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: athotel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripscout/refs/heads/main/security/tripscout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Travel Deals
- Flights
- Hotels
- Consumer
- Media
- Email
- Social
---
