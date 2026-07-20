---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gokite.ai
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: gokite.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: docs.gokite.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: rpc.gokite.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kite
provider_slug: kite
slug: kite-domain-security
source_filename: kite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gokite.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n- host: docs.gokite.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: rpc.gokite.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gokite.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kite/refs/heads/main/security/kite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agentic Payments
- AI Agents
- x402
- Stablecoins
- Blockchain
- EVM
- Layer 1
- Machine-to-Machine
- Identity
- Payments
- JSON-RPC
- Account Abstraction
---
