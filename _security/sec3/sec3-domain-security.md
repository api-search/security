---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sec3.dev
  spf: true
hosts:
- cert_expires: Sep 12 03:58:33 2026 GMT
  host: sec3.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sec3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sec3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sec3
provider_slug: sec3
slug: sec3-domain-security
source_filename: sec3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sec3.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:58:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sec3.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec3/refs/heads/main/security/sec3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Security
- Blockchain
- Solana
- Smart Contracts
- Auditing
- Formal Verification
---
