---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bannerman.com
  spf: true
hosts:
- cert_expires: Aug 23 09:20:44 2026 GMT
  host: bannerman.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bannerman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bannerman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: bannerman
provider_slug: bannerman
slug: bannerman-domain-security
source_filename: bannerman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bannerman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:20:44 2026 GMT\n  hsts: false\ndomains:\n- domain: bannerman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bannerman/refs/heads/main/security/bannerman-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Physical Security
- Security Guards
- Marketplace
- Workforce Management
- Field Services
---
