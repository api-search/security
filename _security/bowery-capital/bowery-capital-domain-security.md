---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bowerycap.com
  spf: true
hosts:
- cert_expires: Sep  9 09:15:10 2026 GMT
  host: bowerycap.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bowery Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bowery Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bowery Capital
provider_slug: bowery-capital
slug: bowery-capital-domain-security
source_filename: bowery-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bowerycap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 09:15:10 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: bowerycap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bowery-capital/refs/heads/main/security/bowery-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venture Capital
- Investor
- Seed
- Pre-Seed
- B2B
- SaaS
- Marketplaces
- Vertical AI
---
