---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parallel.life
  spf: true
hosts:
- cert_expires: Sep 21 10:20:40 2026 GMT
  host: parallel.life
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parallel Universe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parallel Universe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Parallel Universe
provider_slug: parallel-universe
slug: parallel-universe-domain-security
source_filename: parallel-universe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parallel.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:20:40 2026 GMT\n  hsts: false\ndomains:\n- domain: parallel.life\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel-universe/refs/heads/main/security/parallel-universe-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Gaming
- Web3
- Trading Card Game
- Blockchain
- NFT
- Entertainment
- Consumer
---
