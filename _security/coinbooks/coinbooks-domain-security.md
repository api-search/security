---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coinbooks.xyz
  spf: false
hosts:
- cert_expires: Sep 10 02:59:30 2026 GMT
  host: coinbooks.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinbooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinbooks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Coinbooks
provider_slug: coinbooks
slug: coinbooks-domain-security
source_filename: coinbooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinbooks.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 02:59:30 2026 GMT\n  hsts: null\ndomains:\n- domain: coinbooks.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinbooks/refs/heads/main/security/coinbooks-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto Web3
- Blockchain
- Cryptocurrency
- Bookkeeping
---
