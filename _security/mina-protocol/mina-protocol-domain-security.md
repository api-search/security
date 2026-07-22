---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: minaprotocol.com
  spf: true
hosts:
- cert_expires: Aug 28 08:47:09 2026 GMT
  host: minaprotocol.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:06:55 2026 GMT
  host: docs.minaprotocol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mina Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mina Protocol, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mina Protocol
provider_slug: mina-protocol
slug: mina-protocol-domain-security
source_filename: mina-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minaprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:47:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.minaprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:06:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: minaprotocol.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mina-protocol/refs/heads/main/security/mina-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- Zero Knowledge Proofs
- zk-SNARKs
- Smart Contracts
- GraphQL
- Rosetta API
- Developer Tools
---
