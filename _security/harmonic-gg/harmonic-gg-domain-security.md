---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: harmonic.gg
  spf: true
hosts:
- cert_expires: Oct  8 05:57:18 2026 GMT
  host: harmonic.gg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harmonic Gg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harmonic GG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Harmonic GG
provider_slug: harmonic-gg
slug: harmonic-gg-domain-security
source_filename: harmonic-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harmonic.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:57:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: harmonic.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonic-gg/refs/heads/main/security/harmonic-gg-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Blockchain
- Solana
- Block Building
- MEV
- Validator
- Searcher
- Infrastructure
- gRPC
- DeFi
---
