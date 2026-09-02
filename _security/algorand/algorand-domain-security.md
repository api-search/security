---
api_specs:
- filename: algorand-common-api-openapi.yml
  format: yaml
  label: Algorand common API
  slug: algorand-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-common-api-openapi.yml
- filename: algorand-key-api-openapi.yml
  format: yaml
  label: Algorand Key API
  slug: algorand-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-key-api-openapi.yml
- filename: algorand-lookup-api-openapi.yml
  format: yaml
  label: Algorand lookup API
  slug: algorand-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-lookup-api-openapi.yml
- filename: algorand-master-key-api-openapi.yml
  format: yaml
  label: Algorand Master Key API
  slug: algorand-master-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-master-key-api-openapi.yml
- filename: algorand-multisig-api-openapi.yml
  format: yaml
  label: Algorand Multisig API
  slug: algorand-multisig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-multisig-api-openapi.yml
- filename: algorand-private-api-openapi.yml
  format: yaml
  label: Algorand private API
  slug: algorand-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-private-api-openapi.yml
- filename: algorand-program-api-openapi.yml
  format: yaml
  label: Algorand Program API
  slug: algorand-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-program-api-openapi.yml
- filename: algorand-public-api-openapi.yml
  format: yaml
  label: Algorand public API
  slug: algorand-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-public-api-openapi.yml
- filename: algorand-search-api-openapi.yml
  format: yaml
  label: Algorand search API
  slug: algorand-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-search-api-openapi.yml
- filename: algorand-swagger-json-api-openapi.yml
  format: yaml
  label: Algorand Swagger.json API
  slug: algorand-swagger-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-swagger-json-api-openapi.yml
- filename: algorand-transaction-api-openapi.yml
  format: yaml
  label: Algorand Transaction API
  slug: algorand-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-transaction-api-openapi.yml
- filename: algorand-versions-api-openapi.yml
  format: yaml
  label: Algorand Versions API
  slug: algorand-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-versions-api-openapi.yml
- filename: algorand-wallet-api-openapi.yml
  format: yaml
  label: Algorand Wallet API
  slug: algorand-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-wallet-api-openapi.yml
- filename: algorand-wallets-api-openapi.yml
  format: yaml
  label: Algorand Wallets API
  slug: algorand-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-wallets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: algorand.co
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: nodely.dev
  spf: false
hosts:
- cert_expires: Aug 29 18:41:32 2026 GMT
  host: algorand.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 21:19:56 2026 GMT
  host: dev.algorand.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 16:09:24 2026 GMT
  host: mainnet-api.4160.nodely.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Algorand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Algorand, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Algorand
provider_slug: algorand
slug: algorand-domain-security
source_filename: algorand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: algorand.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:41:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.algorand.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:19:56 2026 GMT\n  hsts: false\n- host: mainnet-api.4160.nodely.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:09:24 2026 GMT\n  hsts: false\ndomains:\n- domain: algorand.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nodely.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/security/algorand-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- Proof of Stake
- DeFi
- Smart Contracts
---
