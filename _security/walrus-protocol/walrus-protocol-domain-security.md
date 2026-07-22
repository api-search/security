---
api_specs:
- filename: walrus-protocol-aggregator-openapi.json
  format: json
  label: Walrus Aggregator API
  slug: walrus-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walrus-protocol/refs/heads/main/openapi/walrus-protocol-aggregator-openapi.json
- filename: walrus-protocol-publisher-openapi.json
  format: json
  label: Walrus Publisher API
  slug: walrus-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walrus-protocol/refs/heads/main/openapi/walrus-protocol-publisher-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: walrus.xyz
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wal.app
  spf: false
hosts:
- cert_expires: Aug 22 17:12:55 2026 GMT
  host: www.walrus.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:37:00 2026 GMT
  host: docs.wal.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 14:47:24 2026 GMT
  host: aggregator.walrus-mainnet.walrus.space
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walrus Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walrus Protocol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Walrus Protocol
provider_slug: walrus-protocol
slug: walrus-protocol-domain-security
source_filename: walrus-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.walrus.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:12:55 2026 GMT\n  hsts: false\n- host: docs.wal.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:37:00 2026 GMT\n  hsts: false\n- host: aggregator.walrus-mainnet.walrus.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 14:47:24 2026 GMT\n  hsts: null\ndomains:\n- domain: walrus.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wal.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walrus-protocol/refs/heads/main/security/walrus-protocol-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure
- Storage
- Decentralized Storage
- Blockchain
- Web3
- Data
- AI
- Sui
---
