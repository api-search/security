---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blockfi.com
  spf: true
hosts:
- cert_expires: Nov  5 07:39:52 2026 GMT
  host: blockfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockFi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BlockFi
provider_slug: blockfi
slug: blockfi-domain-security
source_filename: blockfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 07:39:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blockfi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockfi/refs/heads/main/security/blockfi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Digital Assets
- Crypto Lending
- Financial Services
- Fintech
- Blockchain
- Bankruptcy Estate
- Defunct
- United States
---
