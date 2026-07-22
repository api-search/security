---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: virgingalactic.com
  spf: true
hosts:
- cert_expires: Sep 30 06:52:34 2026 GMT
  host: www.virgingalactic.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virgin Galactic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virgin Galactic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Virgin Galactic
provider_slug: virgin-galactic
slug: virgin-galactic-domain-security
source_filename: virgin-galactic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virgingalactic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:52:34 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: virgingalactic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-galactic/refs/heads/main/security/virgin-galactic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Space
- Spaceflight
- Space Tourism
- Aerospace
- Aviation
---
