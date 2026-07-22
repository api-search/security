---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: courtyard.io
  spf: true
hosts:
- cert_expires: Oct  2 02:25:56 2026 GMT
  host: courtyard.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Courtyard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Courtyard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Courtyard
provider_slug: courtyard
slug: courtyard-domain-security
source_filename: courtyard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: courtyard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:25:56 2026 GMT\n  hsts: false\ndomains:\n- domain: courtyard.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/courtyard/refs/heads/main/security/courtyard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Commerce
- Collectibles
- Marketplace
- Tokenization
- NFT
- Blockchain
- Web3
---
