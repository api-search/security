---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drivemate.asia
  spf: true
hosts:
- cert_expires: Aug 23 04:01:52 2026 GMT
  host: drivemate.asia
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drivemate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drivemate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Drivemate
provider_slug: drivemate
slug: drivemate-domain-security
source_filename: drivemate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drivemate.asia\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 04:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: drivemate.asia\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drivemate/refs/heads/main/security/drivemate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Car Sharing
- Car Rental
- Mobility
- Peer-to-Peer
- Marketplace
- Transportation
- Automotive
- Thailand
---
