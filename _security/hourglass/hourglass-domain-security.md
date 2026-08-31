---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hourglass.com
  spf: true
hosts:
- cert_expires: Sep 21 14:27:07 2026 GMT
  host: hourglass.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hourglass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hourglass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hourglass
provider_slug: hourglass
slug: hourglass-domain-security
source_filename: hourglass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hourglass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:27:07 2026 GMT\n  hsts: false\ndomains:\n- domain: hourglass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hourglass/refs/heads/main/security/hourglass-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Defi
- Blockchain
- Ethereum
- Tokenization
- Yield
- Marketplace
- Smart Contracts
- Web3
---
