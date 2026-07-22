---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quickride.in
  spf: true
hosts:
- cert_expires: Sep 20 07:47:23 2026 GMT
  host: quickride.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quick Ride Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quick Ride, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quick Ride
provider_slug: quick-ride
slug: quick-ride-domain-security
source_filename: quick-ride-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickride.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 07:47:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quickride.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quick-ride/refs/heads/main/security/quick-ride-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobility
- Ride Sharing
- Carpooling
- Bikepool
- Taxi
- Transportation
- India
---
