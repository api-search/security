---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fbg.capital
  spf: true
hosts:
- cert_expires: Sep 19 10:49:18 2026 GMT
  host: fbg.capital
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fbg Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FBG Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FBG Capital
provider_slug: fbg-capital
slug: fbg-capital-domain-security
source_filename: fbg-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fbg.capital\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 10:49:18 2026 GMT\n  hsts: false\ndomains:\n- domain: fbg.capital\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fbg-capital/refs/heads/main/security/fbg-capital-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Investment
- Venture Capital
- Blockchain
- Cryptocurrency
- Digital Assets
- Web3
- DeFi
---
