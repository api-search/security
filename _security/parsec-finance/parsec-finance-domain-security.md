---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parsec.fi
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: parsec.finance
  spf: true
hosts:
- cert_expires: Sep  7 23:16:10 2026 GMT
  host: parsec.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 00:16:09 2026 GMT
  host: docs.parsec.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 00:16:09 2026 GMT
  host: api.parsec.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parsec Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsec Finance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Parsec Finance
provider_slug: parsec-finance
slug: parsec-finance-domain-security
source_filename: parsec-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parsec.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:16:10 2026 GMT\n  hsts: null\n- host: docs.parsec.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:16:09 2026 GMT\n  hsts: null\n- host: api.parsec.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:16:09 2026 GMT\n  hsts: null\ndomains:\n- domain: parsec.fi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: parsec.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsec-finance/refs/heads/main/security/parsec-finance-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Analytics
- DeFi
- NFT
- Blockchain
- Cryptocurrency
- On-Chain Data
- Web3
- GraphQL
- Trading
---
