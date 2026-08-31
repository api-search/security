---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sandbox.game
  spf: true
hosts:
- cert_expires: Oct  3 01:00:32 2026 GMT
  host: www.sandbox.game
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 22:15:38 2026 GMT
  host: developers.sandbox.game
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Sand Box Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Sandbox, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Sandbox
provider_slug: the-sand-box
slug: the-sand-box-domain-security
source_filename: the-sand-box-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sandbox.game\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:00:32 2026 GMT\n  hsts: null\n- host: developers.sandbox.game\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 22:15:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sandbox.game\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-sand-box/refs/heads/main/security/the-sand-box-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Metaverse
- Gaming
- Blockchain
- NFT
- Web3
- Virtual Worlds
- User Generated Content
- Ethereum
- Identity
---
