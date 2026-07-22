---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unbound.finance
  spf: true
hosts:
- cert_expires: Sep  4 06:44:47 2026 GMT
  host: www.unbound.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unbound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unbound, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unbound
provider_slug: unbound
slug: unbound-domain-security
source_filename: unbound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unbound.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 06:44:47 2026 GMT\n  hsts: null\ndomains:\n- domain: unbound.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbound/refs/heads/main/security/unbound-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- DeFi
- Liquidity
- Ethereum
- Venture Portfolio
---
