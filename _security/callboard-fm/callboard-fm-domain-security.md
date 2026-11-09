---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: callboard.fm
  spf: false
hosts:
- cert_expires: Dec 12 15:00:18 2026 GMT
  host: callboard.fm
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Callboard Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Callboard.fm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Callboard.fm
provider_slug: callboard-fm
slug: callboard-fm-domain-security
source_filename: callboard-fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callboard.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:00:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: callboard.fm\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/callboard-fm/security/callboard-fm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Concerts
- Booking
- Intelligence
- Promoters
---
