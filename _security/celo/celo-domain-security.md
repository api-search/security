---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: celo.org
  spf: true
hosts:
- cert_expires: Aug 21 00:23:00 2026 GMT
  host: celo.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Celo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Celo
provider_slug: celo
slug: celo-domain-security
source_filename: celo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:23:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: celo.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celo/refs/heads/main/security/celo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Ethereum L2
- Web3
- Stablecoins
- Payments
- JSON-RPC
- Smart Contracts
- AI Agents
- Developer Tools
---
