---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coreloop.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: coreloop.gg
  spf: false
hosts:
- cert_expires: Sep 12 14:16:23 2026 GMT
  host: coreloop.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 04:53:29 2026 GMT
  host: coreloop.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Core Loop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Core Loop, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Core Loop
provider_slug: core-loop
slug: core-loop-domain-security
source_filename: core-loop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coreloop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 14:16:23 2026 GMT\n  hsts: false\n- host: coreloop.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:53:29 2026 GMT\n  hsts: false\ndomains:\n- domain: coreloop.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: coreloop.gg\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/core-loop/refs/heads/main/security/core-loop-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Games
- Gaming
- Game Studio
- MMO
- Web3
- Blockchain
- NFT
- Virtual Economy
- AI
---
