---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: superfluid.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: superfluid.dev
  spf: true
hosts:
- cert_expires: Aug 25 04:15:13 2026 GMT
  host: www.superfluid.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 22:25:01 2026 GMT
  host: docs.superfluid.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: subgraph-endpoints.superfluid.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superfluid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superfluid, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Superfluid
provider_slug: superfluid
slug: superfluid-domain-security
source_filename: superfluid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superfluid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 04:15:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.superfluid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:25:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: subgraph-endpoints.superfluid.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: superfluid.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: superfluid.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superfluid/refs/heads/main/security/superfluid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- DeFi
- Payments
- Money Streaming
- Ethereum
- GraphQL
- Smart Contracts
---
