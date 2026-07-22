---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: team8.vc
  spf: true
hosts:
- cert_expires: Oct  9 08:18:41 2026 GMT
  host: www.team8.vc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Team8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Team8, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Team8
provider_slug: team8
slug: team8-domain-security
source_filename: team8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.team8.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: team8.vc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/team8/refs/heads/main/security/team8-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Software Infrastructure
- Fintech
- Digital Health
- Venture Capital
- Venture Creation
- Company Builder
- Israel
---
