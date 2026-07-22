---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fastlane.xyz
  spf: true
hosts:
- cert_expires: Oct 15 07:00:25 2026 GMT
  host: fastlane.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fastlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FastLane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FastLane
provider_slug: fastlane
slug: fastlane-domain-security
source_filename: fastlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastlane.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 07:00:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fastlane.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastlane/refs/heads/main/security/fastlane-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto Web3
- Blockchain
- MEV
- Liquid Staking
- DeFi
- Monad
- Staking
- JSON-RPC
---
