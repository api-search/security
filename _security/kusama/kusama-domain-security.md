---
api_specs:
- filename: kusama-jsonrpc-asyncapi.yml
  format: yaml
  label: Kusama JSON-RPC API
  slug: json-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/asyncapi/kusama-jsonrpc-asyncapi.yml
- filename: kusama-accounts-api-openapi.yml
  format: yaml
  label: Kusama accounts API
  slug: kusama-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-accounts-api-openapi.yml
- filename: kusama-ahm-api-openapi.yml
  format: yaml
  label: Kusama ahm API
  slug: kusama-ahm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-ahm-api-openapi.yml
- filename: kusama-blocks-api-openapi.yml
  format: yaml
  label: Kusama blocks API
  slug: kusama-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-blocks-api-openapi.yml
- filename: kusama-contracts-api-openapi.yml
  format: yaml
  label: Kusama contracts API
  slug: kusama-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-contracts-api-openapi.yml
- filename: kusama-coretime-api-openapi.yml
  format: yaml
  label: Kusama coretime API
  slug: kusama-coretime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-coretime-api-openapi.yml
- filename: kusama-node-api-openapi.yml
  format: yaml
  label: Kusama node API
  slug: kusama-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-node-api-openapi.yml
- filename: kusama-pallets-api-openapi.yml
  format: yaml
  label: Kusama pallets API
  slug: kusama-pallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-pallets-api-openapi.yml
- filename: kusama-paras-api-openapi.yml
  format: yaml
  label: Kusama paras API
  slug: kusama-paras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-paras-api-openapi.yml
- filename: kusama-rc-accounts-api-openapi.yml
  format: yaml
  label: Kusama rc accounts API
  slug: kusama-rc-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-rc-accounts-api-openapi.yml
- filename: kusama-rc-api-openapi.yml
  format: yaml
  label: Kusama rc API
  slug: kusama-rc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-rc-api-openapi.yml
- filename: kusama-rc-blocks-api-openapi.yml
  format: yaml
  label: Kusama rc blocks API
  slug: kusama-rc-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-rc-blocks-api-openapi.yml
- filename: kusama-rc-node-api-openapi.yml
  format: yaml
  label: Kusama rc node API
  slug: kusama-rc-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-rc-node-api-openapi.yml
- filename: kusama-rc-pallets-api-openapi.yml
  format: yaml
  label: Kusama rc pallets API
  slug: kusama-rc-pallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-rc-pallets-api-openapi.yml
- filename: kusama-rc-runtime-api-openapi.yml
  format: yaml
  label: Kusama rc runtime API
  slug: kusama-rc-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-rc-runtime-api-openapi.yml
- filename: kusama-rc-staking-api-openapi.yml
  format: yaml
  label: Kusama rc staking API
  slug: kusama-rc-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-rc-staking-api-openapi.yml
- filename: kusama-rc-transaction-api-openapi.yml
  format: yaml
  label: Kusama rc transaction API
  slug: kusama-rc-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-rc-transaction-api-openapi.yml
- filename: kusama-runtime-api-openapi.yml
  format: yaml
  label: Kusama runtime API
  slug: kusama-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-runtime-api-openapi.yml
- filename: kusama-staking-api-openapi.yml
  format: yaml
  label: Kusama staking API
  slug: kusama-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-staking-api-openapi.yml
- filename: kusama-trace-api-openapi.yml
  format: yaml
  label: Kusama trace API
  slug: kusama-trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-trace-api-openapi.yml
- filename: kusama-transaction-api-openapi.yml
  format: yaml
  label: Kusama transaction API
  slug: kusama-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/openapi/kusama-transaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kusama.network
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "security@parity.io"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: polkadot.io
  spf: true
hosts:
- cert_expires: Oct  2 11:13:48 2026 GMT
  host: kusama.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 03:34:54 2026 GMT
  host: kusama-rpc.polkadot.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:06:46 2026 GMT
  host: docs.polkadot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kusama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kusama, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kusama
provider_slug: kusama
slug: kusama-domain-security
source_filename: kusama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kusama.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kusama-rpc.polkadot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:34:54 2026 GMT\n  hsts: null\n- host: docs.polkadot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:06:46 2026 GMT\n  hsts: false\ndomains:\n- domain: kusama.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: polkadot.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"security@parity.io\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kusama/refs/heads/main/security/kusama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- Web3
- Polkadot
- Substrate
- JSON-RPC
- Blockchain Data
- Staking
- Governance
---
