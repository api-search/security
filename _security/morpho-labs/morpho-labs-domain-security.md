---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: morpho.org
  spf: true
hosts:
- cert_expires: Sep 23 09:03:13 2026 GMT
  host: morpho.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 18:54:39 2026 GMT
  host: docs.morpho.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.morpho.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morpho Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morpho Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Morpho Labs
provider_slug: morpho-labs
slug: morpho-labs-domain-security
source_filename: morpho-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morpho.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:03:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.morpho.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:54:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.morpho.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: morpho.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morpho-labs/refs/heads/main/security/morpho-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- DeFi
- Lending
- Blockchain
- Ethereum
- GraphQL
- Onchain Data
- Financial Services
- Web3
- Crypto
---
