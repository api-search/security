---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: communitygaming.io
  spf: true
hosts:
- cert_expires: Oct  8 03:51:07 2026 GMT
  host: communitygaming.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Community Gaming Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Community Gaming, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Community Gaming
provider_slug: community-gaming
slug: community-gaming-domain-security
source_filename: community-gaming-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: communitygaming.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:51:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: communitygaming.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community-gaming/refs/heads/main/security/community-gaming-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Gaming
- Esports
- Tournaments
- Rewards
- Web3
- Blockchain
---
