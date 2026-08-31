---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mezo.org
  spf: true
hosts:
- cert_expires: Oct 17 11:05:04 2026 GMT
  host: mezo.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mezo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mezo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mezo
provider_slug: mezo
slug: mezo-domain-security
source_filename: mezo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mezo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:05:04 2026 GMT\n  hsts: false\ndomains:\n- domain: mezo.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mezo/refs/heads/main/security/mezo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- Bitcoin
- DeFi
- EVM
- Cosmos SDK
- Stablecoin
- JSON-RPC
- Layer 2
---
