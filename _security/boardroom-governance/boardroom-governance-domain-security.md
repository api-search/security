---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boardroom.io
  spf: true
hosts:
- cert_expires: Aug 29 20:53:51 2026 GMT
  host: boardroom.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 16:09:44 2026 GMT
  host: docs.boardroom.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boardroom Governance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boardroom Governance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Boardroom Governance
provider_slug: boardroom-governance
slug: boardroom-governance-domain-security
source_filename: boardroom-governance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boardroom.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:53:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.boardroom.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:09:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boardroom.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boardroom-governance/refs/heads/main/security/boardroom-governance-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Blockchain
- Governance
- DAO
- Web3
- Decentralized
---
