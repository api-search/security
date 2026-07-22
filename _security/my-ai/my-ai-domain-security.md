---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meprotocol.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: pages.dev
  spf: false
hosts:
- cert_expires: Sep 15 05:33:18 2026 GMT
  host: meprotocol.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 12:58:46 2026 GMT
  host: me-api-docs.pages.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: paas.memarketplace.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: My Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for My AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: My AI
provider_slug: my-ai
slug: my-ai-domain-security
source_filename: my-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meprotocol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:33:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: me-api-docs.pages.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 12:58:46 2026 GMT\n  hsts: false\n- host: paas.memarketplace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: meprotocol.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: pages.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/my-ai/refs/heads/main/security/my-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Rewards
- Loyalty
- Web3
- Blockchain
- API
- SDK
- AI Agent
- Payments
- Smart Contracts
---
