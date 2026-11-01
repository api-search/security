---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pinboard.in
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: pinboard.in
  hsts: true
  hsts_max_age: 1607000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pinboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pinboard
provider_slug: pinboard
slug: pinboard-domain-security
source_filename: pinboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pinboard.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 1607000\ndomains:\n- domain: pinboard.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pinboard/security/pinboard-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Bookmarking
- Social
- API
- Productivity
- Web
---
