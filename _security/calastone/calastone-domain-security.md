---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: calastone.com
  spf: true
hosts:
- cert_expires: Aug 19 19:25:39 2026 GMT
  host: www.calastone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calastone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calastone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Calastone
provider_slug: calastone
slug: calastone-domain-security
source_filename: calastone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.calastone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:25:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: calastone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calastone/refs/heads/main/security/calastone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Funds
- Asset Management
- Fund Administration
- Financial Services
- Money Markets
- Settlements
- Tokenization
---
