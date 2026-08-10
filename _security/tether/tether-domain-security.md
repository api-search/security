---
api_specs:
- filename: tether-api-keys-api-openapi.yml
  format: yaml
  label: Tether API Keys API
  slug: tether-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-api-keys-api-openapi.yml
- filename: tether-chains-api-openapi.yml
  format: yaml
  label: Tether Chains API
  slug: tether-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-chains-api-openapi.yml
- filename: tether-health-api-openapi.yml
  format: yaml
  label: Tether Health API
  slug: tether-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-health-api-openapi.yml
- filename: tether-token-balances-api-openapi.yml
  format: yaml
  label: Tether Token Balances API
  slug: tether-token-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-token-balances-api-openapi.yml
- filename: tether-token-transfers-api-openapi.yml
  format: yaml
  label: Tether Token Transfers API
  slug: tether-token-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/openapi/tether-token-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tether.io
  spf: true
hosts:
- cert_expires: Oct 22 11:37:05 2026 GMT
  host: tether.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 11:35:07 2026 GMT
  host: docs.wdk.tether.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 11:37:05 2026 GMT
  host: wdk-api.tether.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tether Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tether, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tether
provider_slug: tether
slug: tether-domain-security
source_filename: tether-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tether.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 11:37:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.wdk.tether.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:35:07 2026 GMT\n  hsts: false\n- host: wdk-api.tether.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 11:37:05 2026 GMT\n  hsts: null\ndomains:\n- domain: tether.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tether/refs/heads/main/security/tether-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stablecoins
- Cryptocurrency
- Blockchain
- Wallets
- Digital Assets
- Payments
- Self-Custody
- Multi-Chain
- Agents
- MCP
- Open Source
---
