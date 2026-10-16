---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theplayerstrunk.com
  spf: true
hosts:
- cert_expires: Dec 26 15:37:31 2026 GMT
  host: theplayerstrunk.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Players Trunk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Players Trunk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Players Trunk
provider_slug: the-players-trunk
slug: the-players-trunk-domain-security
source_filename: the-players-trunk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theplayerstrunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 15:37:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: theplayerstrunk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-players-trunk/refs/heads/main/security/the-players-trunk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Sports
- Apparel
- WeeklyDrops
---
