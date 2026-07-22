---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: placeholder.vc
  spf: true
hosts:
- cert_expires: Oct 18 04:55:48 2026 GMT
  host: www.placeholder.vc
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Placeholder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Placeholder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Placeholder
provider_slug: placeholder
slug: placeholder-domain-security
source_filename: placeholder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.placeholder.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 04:55:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: placeholder.vc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/placeholder/refs/heads/main/security/placeholder-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Venture Capital
- Crypto
- Web3
- Blockchain
- Decentralization
---
