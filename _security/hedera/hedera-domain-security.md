---
api_specs:
- filename: swagger.json
  format: json
  label: Hedera Mirror Node REST API
  slug: hedera-mirror-node-rest-api
  spec_type: OpenAPI
  url: https://mainnet.mirrornode.hedera.com/api/v1/docs/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hedera.com
  spf: true
hosts:
- cert_expires: Aug 26 15:59:11 2026 GMT
  host: portal.hedera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 17:25:19 2026 GMT
  host: docs.hedera.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 03:42:55 2026 GMT
  host: mainnet.mirrornode.hedera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hedera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hedera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hedera
provider_slug: hedera
slug: hedera-domain-security
source_filename: hedera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.hedera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 15:59:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hedera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mainnet.mirrornode.hedera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 03:42:55 2026 GMT\n  hsts: null\ndomains:\n- domain: hedera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hedera/refs/heads/main/security/hedera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Distributed Ledger
- Blockchain
- DLT
- Hashgraph
- Transactions
- Tokens
- NFTs
- Smart Contracts
- Enterprise
---
