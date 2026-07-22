---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: nvolume.com
  spf: true
hosts:
- cert_expires: Sep 23 13:48:37 2026 GMT
  host: nvolume.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: And Volume Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for &Volume, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: '&Volume'
provider_slug: and-volume
slug: and-volume-domain-security
source_filename: and-volume-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nvolume.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 13:48:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nvolume.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/and-volume/refs/heads/main/security/and-volume-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Company
- Digital Assets
- Risk Management
- Cryptocurrency
- Institutional Investing
- FinTech
- Artificial Intelligence
- Portfolio Management
- Blockchain
- Treasury Management
---
