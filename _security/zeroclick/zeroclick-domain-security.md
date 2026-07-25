---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zeroclick.ai
  spf: true
hosts:
- cert_expires: Aug 27 18:29:15 2026 GMT
  host: zeroclick.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeroclick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeroclick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zeroclick
provider_slug: zeroclick
slug: zeroclick-domain-security
source_filename: zeroclick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeroclick.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:29:15 2026 GMT\n  hsts: false\ndomains:\n- domain: zeroclick.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeroclick/refs/heads/main/security/zeroclick-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Agent Commerce
- Agentic Payments
- API Monetization
- x402
- Machine Payments Protocol
- Agent Identity
- Stripe
---
