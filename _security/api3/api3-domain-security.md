---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: api3.org
  spf: true
hosts:
- cert_expires: Sep 15 01:55:15 2026 GMT
  host: api3.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 22:22:21 2026 GMT
  host: market.api3.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 02:42:23 2026 GMT
  host: docs.api3.org
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API3, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: API3
provider_slug: api3
slug: api3-domain-security
source_filename: api3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:55:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: market.api3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 22:22:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.api3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:42:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: api3.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api3/refs/heads/main/security/api3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Oracle
- Decentralized
- Data Feeds
- Price Feeds
- Web3
- DeFi
- Smart Contracts
- OEV
- dAPI
---
