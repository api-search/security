---
api_specs:
- filename: zksync-asyncapi.yml
  format: yaml
  label: zkSync Era WebSocket
  slug: era-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zksync/refs/heads/main/asyncapi/zksync-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zksync.io
  spf: true
hosts:
- cert_expires: Sep 26 14:03:09 2026 GMT
  host: zksync.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 17:32:24 2026 GMT
  host: portal.zksync.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:47:34 2026 GMT
  host: docs.zksync.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zksync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zkSync, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: zkSync
provider_slug: zksync
slug: zksync-domain-security
source_filename: zksync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zksync.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:03:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.zksync.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:32:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.zksync.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:47:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: zksync.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zksync/refs/heads/main/security/zksync-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Layer 2
- Ethereum
- zkEVM
- ZK Rollup
- Account Abstraction
- Paymaster
- ZK Stack
- Bridge
---
