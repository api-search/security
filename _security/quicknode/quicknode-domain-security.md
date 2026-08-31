---
api_specs:
- filename: quicknode-asyncapi.yml
  format: yaml
  label: QuickNode Core RPC API
  slug: core-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/asyncapi/quicknode-asyncapi.yml
- filename: quicknode-account-api-openapi.yml
  format: yaml
  label: QuickNode Account API
  slug: quicknode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-account-api-openapi.yml
- filename: quicknode-batch-api-openapi.yml
  format: yaml
  label: QuickNode Batch API
  slug: quicknode-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-batch-api-openapi.yml
- filename: quicknode-database-api-openapi.yml
  format: yaml
  label: QuickNode Database API
  slug: quicknode-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-database-api-openapi.yml
- filename: quicknode-gateway-api-openapi.yml
  format: yaml
  label: QuickNode Gateway API
  slug: quicknode-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-gateway-api-openapi.yml
- filename: quicknode-keys-api-openapi.yml
  format: yaml
  label: QuickNode Keys API
  slug: quicknode-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-keys-api-openapi.yml
- filename: quicknode-logs-api-openapi.yml
  format: yaml
  label: QuickNode Logs API
  slug: quicknode-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-logs-api-openapi.yml
- filename: quicknode-pinning-api-openapi.yml
  format: yaml
  label: QuickNode Pinning API
  slug: quicknode-pinning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-pinning-api-openapi.yml
- filename: quicknode-streams-api-openapi.yml
  format: yaml
  label: QuickNode Streams API
  slug: quicknode-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-streams-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quicknode.com
  spf: true
hosts:
- cert_expires: Aug 27 19:44:18 2026 GMT
  host: www.quicknode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 19:44:18 2026 GMT
  host: api.quicknode.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 19:44:18 2026 GMT
  host: marketplace.quicknode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quicknode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuickNode, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: QuickNode
provider_slug: quicknode
slug: quicknode-domain-security
source_filename: quicknode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quicknode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:44:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.quicknode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:44:18 2026 GMT\n  hsts: null\n- host: marketplace.quicknode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:44:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quicknode.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/security/quicknode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Blockchain
- RPC
- Streams
- IPFS
- Multi-chain
---
