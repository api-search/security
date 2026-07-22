---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lawtrades.com
  spf: true
hosts:
- cert_expires: Sep 11 22:10:02 2026 GMT
  host: lawtrades.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lawtrades Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LawTrades, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LawTrades
provider_slug: lawtrades
slug: lawtrades-domain-security
source_filename: lawtrades-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lawtrades.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 22:10:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lawtrades.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lawtrades/refs/heads/main/security/lawtrades-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Services
- Legal Operations
- Marketplace
- Talent Marketplace
- Contracts
- Compliance
- Professional Services
- Artificial Intelligence
---
