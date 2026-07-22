---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ob1.io
  spf: true
hosts:
- cert_expires: Sep  1 17:47:37 2026 GMT
  host: ob1.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ob1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OB1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: OB1
provider_slug: ob1
slug: ob1-domain-security
source_filename: ob1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ob1.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:47:37 2026 GMT\n  hsts: null\ndomains:\n- domain: ob1.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ob1/refs/heads/main/security/ob1-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Marketplace
- Decentralized
- Cryptocurrency
- Bitcoin
- Peer-to-Peer
- E-commerce
- Blockchain
- Open Source
---
