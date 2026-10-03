---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fly.dev
  spf: false
hosts:
- cert_expires: Nov 19 11:49:32 2026 GMT
  host: rugshield-x402.fly.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rugshield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RugShield Solana Safety API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RugShield Solana Safety API
provider_slug: rugshield
slug: rugshield-domain-security
source_filename: rugshield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rugshield-x402.fly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 11:49:32 2026 GMT\n  hsts: null\ndomains:\n- domain: fly.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rugshield/refs/heads/main/security/rugshield-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Solana
- Risk Management
- Payments
- Artificial Intelligence
---
