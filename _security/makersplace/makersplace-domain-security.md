---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: makersplace.com
  spf: false
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: makersplace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Makersplace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MakersPlace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MakersPlace
provider_slug: makersplace
slug: makersplace-domain-security
source_filename: makersplace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makersplace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: makersplace.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makersplace/refs/heads/main/security/makersplace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- NFT
- Digital Art
- Marketplace
- Blockchain
- Web3
- Art
---
