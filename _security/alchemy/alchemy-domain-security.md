---
api_specs:
- filename: alchemy-asyncapi.yml
  format: yaml
  label: Alchemy Node API (JSON-RPC)
  slug: node-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/asyncapi/alchemy-asyncapi.yml
- filename: alchemy-token-api-openapi.yml
  format: yaml
  label: Alchemy Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/openapi/alchemy-token-api-openapi.yml
- filename: alchemy-transfers-api-openapi.yml
  format: yaml
  label: Alchemy Transfers API
  slug: transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/openapi/alchemy-transfers-api-openapi.yml
- filename: alchemy-gas-manager-api-openapi.yml
  format: yaml
  label: Alchemy Gas Manager API
  slug: gas-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/openapi/alchemy-gas-manager-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alchemy.com
  spf: true
hosts:
- cert_expires: Sep 28 14:11:51 2026 GMT
  host: www.alchemy.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:11:51 2026 GMT
  host: dashboard.alchemy.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 11:37:21 2026 GMT
  host: manage.g.alchemy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alchemy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alchemy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alchemy
provider_slug: alchemy
slug: alchemy-domain-security
source_filename: alchemy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alchemy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:11:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: dashboard.alchemy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:11:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: manage.g.alchemy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:37:21 2026 GMT\n  hsts: null\ndomains:\n- domain: alchemy.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/security/alchemy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Blockchain
- RPC
- NFT
- Indexing
- Account Abstraction
---
