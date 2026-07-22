---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: roller.software
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roller.app
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.roller.software
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 17:04:20 2026 GMT
  host: docs.roller.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.roller.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ROLLER, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ROLLER
provider_slug: roller
slug: roller-domain-security
source_filename: roller-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roller.software\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.roller.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 17:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.roller.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: roller.software\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: roller.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roller/refs/heads/main/security/roller-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venue Management
- Attractions
- Ticketing
- Bookings
- Point of Sale
- Payments
- Leisure
- Reservations
- Webhooks
---
