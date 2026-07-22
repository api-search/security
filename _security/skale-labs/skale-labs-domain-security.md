---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: skale.space
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: skalenodes.com
  spf: false
hosts:
- cert_expires: Aug 19 11:19:47 2026 GMT
  host: skale.space
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:41:51 2026 GMT
  host: docs.skale.space
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 22 11:03:45 2026 GMT
  host: skale-base.skalenodes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skale Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skale Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Skale Labs
provider_slug: skale-labs
slug: skale-labs-domain-security
source_filename: skale-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skale.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 11:19:47 2026 GMT\n  hsts: null\n- host: docs.skale.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:41:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: skale-base.skalenodes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 22 11:03:45 2026 GMT\n  hsts: null\ndomains:\n- domain: skale.space\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: skalenodes.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skale-labs/refs/heads/main/security/skale-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Web3
- Smart Contracts
- Developer Tools
- JSON-RPC
- AI Agents
- Privacy
- Payments
- Cryptocurrency
---
