---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: farcaster.xyz
  spf: true
hosts:
- cert_expires: Sep 16 03:07:29 2026 GMT
  host: snapchain.farcaster.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Merkle Manufactory Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merkle Manufactory Inc., probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Merkle Manufactory Inc.
provider_slug: merkle-manufactory-inc
slug: merkle-manufactory-inc-domain-security
source_filename: merkle-manufactory-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapchain.farcaster.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 03:07:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: farcaster.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merkle-manufactory-inc/refs/heads/main/security/merkle-manufactory-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Social
- Decentralized Social
- Protocol
- Blockchain
- Web3
- Developer Platform
- Farcaster
---
