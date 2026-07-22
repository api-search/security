---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: string.xyz
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: string-api.xyz
  spf: false
hosts:
- host: string.xyz
  https: false
- cert_expires: Sep 15 10:47:45 2026 GMT
  host: docs.string.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: string-api.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: String Technology Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for String Technology Inc, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: String Technology Inc
provider_slug: string-technology-inc
slug: string-technology-inc-domain-security
source_filename: string-technology-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: string.xyz\n  https: false\n- host: docs.string.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:47:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: string-api.xyz\n  https: false\ndomains:\n- domain: string.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: string-api.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/string-technology-inc/refs/heads/main/security/string-technology-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Payments
- Web3
- Gaming
- Fiat On-Ramp
- Cryptocurrency
- NFT
- Merchant of Record
- Developer Tools
---
