---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: archblock.com
  spf: true
hosts:
- cert_expires: Oct 11 01:01:13 2026 GMT
  host: www.archblock.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trust Token Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trust Token, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trust Token
provider_slug: trust-token
slug: trust-token-domain-security
source_filename: trust-token-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.archblock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 01:01:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: archblock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trust-token/refs/heads/main/security/trust-token-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stablecoins
- DeFi
- Blockchain
- Tokenization
- Lending
- Cryptocurrency
- FinTech
---
