---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: brightmoments.io
  spf: true
hosts:
- cert_expires: Aug 18 21:58:57 2026 GMT
  host: www.brightmoments.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bright Moments Dao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Moments DAO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Bright Moments DAO
provider_slug: bright-moments-dao
slug: bright-moments-dao-domain-security
source_filename: bright-moments-dao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightmoments.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:58:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: brightmoments.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-moments-dao/refs/heads/main/security/bright-moments-dao-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- NFT
- DAO
- Generative Art
- Web3
- Ethereum
- Smart Contracts
- Digital Art
- Governance
---
