---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mockko.com
  spf: true
hosts:
- cert_expires: Dec 15 06:49:50 2026 GMT
  host: mockko.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mockko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mockko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mockko
provider_slug: mockko
slug: mockko-domain-security
source_filename: mockko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mockko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 06:49:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mockko.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mockko/refs/heads/main/security/mockko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dashboard
- Mockup
- PowerBI
- Tableau
- Design
---
