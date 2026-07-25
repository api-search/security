---
api_specs:
- filename: iota-auth-api-openapi.yml
  format: yaml
  label: IOTA auth API
  slug: iota-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-auth-api-openapi.yml
- filename: iota-chains-api-openapi.yml
  format: yaml
  label: IOTA chains API
  slug: iota-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-chains-api-openapi.yml
- filename: iota-coin-query-api-openapi.yml
  format: yaml
  label: IOTA Coin Query API
  slug: iota-coin-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-coin-query-api-openapi.yml
- filename: iota-corecontracts-api-openapi.yml
  format: yaml
  label: IOTA corecontracts API
  slug: iota-corecontracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-corecontracts-api-openapi.yml
- filename: iota-extended-api-openapi.yml
  format: yaml
  label: IOTA Extended API
  slug: iota-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-extended-api-openapi.yml
- filename: iota-governance-api-openapi.yml
  format: yaml
  label: IOTA Governance API
  slug: iota-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-governance-api-openapi.yml
- filename: iota-health-api-openapi.yml
  format: yaml
  label: IOTA Health API
  slug: iota-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-health-api-openapi.yml
- filename: iota-metrics-api-openapi.yml
  format: yaml
  label: IOTA metrics API
  slug: iota-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-metrics-api-openapi.yml
- filename: iota-move-utils-api-openapi.yml
  format: yaml
  label: IOTA Move Utils API
  slug: iota-move-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-move-utils-api-openapi.yml
- filename: iota-node-api-openapi.yml
  format: yaml
  label: IOTA node API
  slug: iota-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-node-api-openapi.yml
- filename: iota-read-api-openapi.yml
  format: yaml
  label: IOTA Read API
  slug: iota-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-read-api-openapi.yml
- filename: iota-requests-api-openapi.yml
  format: yaml
  label: IOTA requests API
  slug: iota-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-requests-api-openapi.yml
- filename: iota-transaction-builder-api-openapi.yml
  format: yaml
  label: IOTA Transaction Builder API
  slug: iota-transaction-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-transaction-builder-api-openapi.yml
- filename: iota-users-api-openapi.yml
  format: yaml
  label: IOTA users API
  slug: iota-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-users-api-openapi.yml
- filename: iota-write-api-openapi.yml
  format: yaml
  label: IOTA Write API
  slug: iota-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-write-api-openapi.yml
- filename: iota-ws-api-openapi.yml
  format: yaml
  label: IOTA Ws API
  slug: iota-ws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-ws-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: iota.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: iota.cafe
  spf: false
hosts:
- cert_expires: Sep 29 01:13:18 2026 GMT
  host: www.iota.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 01:13:18 2026 GMT
  host: docs.iota.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 02:59:25 2026 GMT
  host: api.mainnet.iota.cafe
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iota Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IOTA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: IOTA
provider_slug: iota
slug: iota-domain-security
source_filename: iota-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iota.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:13:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.iota.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:13:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mainnet.iota.cafe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:59:25 2026 GMT\n  hsts: null\ndomains:\n- domain: iota.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: iota.cafe\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/security/iota-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Distributed Ledger
- Web3
- DeFi
- Cryptocurrency
- Move
- Tangle
---
