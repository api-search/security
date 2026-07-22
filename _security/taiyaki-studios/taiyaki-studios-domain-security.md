---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: taiyakistudios.com
  spf: true
hosts:
- cert_expires: Oct  9 21:12:44 2026 GMT
  host: www.taiyakistudios.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taiyaki Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taiyaki Studios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Taiyaki Studios
provider_slug: taiyaki-studios
slug: taiyaki-studios-domain-security
source_filename: taiyaki-studios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.taiyakistudios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 21:12:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taiyakistudios.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taiyaki-studios/refs/heads/main/security/taiyaki-studios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Anime
- Web3
- NFT
- DeFi
- Entertainment
- Content
- Tokyo
---
