---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: maquoketa.net
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
hosts:
- cert_expires: '2026-10-07'
  host: www.maquoketa.net
  hsts: false
  hsts_max_age: null
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- host: maquoketa.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maquoketa Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maquoketa Research, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Maquoketa Research
provider_slug: maquoketa-research
slug: maquoketa-research-domain-security
source_filename: maquoketa-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live TLS/HTTP HEAD + dig on maquoketa.net hosts\nhosts:\n  - host: www.maquoketa.net\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: '2026-10-07'\n    hsts: false\n    hsts_max_age: null\n    server: cloudflare\n  - host: maquoketa.net\n    https: true\n    tls_version: TLSv1.3\n    hsts: false\ndomains:\n  - domain: maquoketa.net\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: v=spf1 include:spf.protection.outlook.com -all\n    dmarc: false\n    dmarc_policy: null\nnotes: >-\n  No DNSSEC (no DS record), no CAA policy, and no DMARC record published as of\n  the probe date. SPF is published for Microsoft 365 / Outlook mail. Site is\n  served behind Cloudflare.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maquoketa-research/refs/heads/main/security/maquoketa-research-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Defense
- Drones
- Autonomous Systems
- Guidance Systems
- Computer Vision
- Hardware
- Aerospace
- Y Combinator
---
