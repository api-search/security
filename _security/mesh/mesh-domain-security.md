---
api_specs:
- filename: mesh-assets-api-openapi.yml
  format: yaml
  label: Mesh Assets API
  slug: mesh-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-assets-api-openapi.yml
- filename: mesh-balance-api-openapi.yml
  format: yaml
  label: Mesh Balance API
  slug: mesh-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-balance-api-openapi.yml
- filename: mesh-brokeraccountdetail-api-openapi.yml
  format: yaml
  label: Mesh BrokerAccountDetail API
  slug: mesh-brokeraccountdetail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-brokeraccountdetail-api-openapi.yml
- filename: mesh-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Managed Account Authentication API
  slug: mesh-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-managed-account-authentication-api-openapi.yml
- filename: mesh-managed-transfers-api-openapi.yml
  format: yaml
  label: Mesh Managed Transfers API
  slug: mesh-managed-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-managed-transfers-api-openapi.yml
- filename: mesh-portfolio-api-openapi.yml
  format: yaml
  label: Mesh Portfolio API
  slug: mesh-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-portfolio-api-openapi.yml
- filename: mesh-self-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Self Managed Account Authentication API
  slug: mesh-self-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-self-managed-account-authentication-api-openapi.yml
- filename: mesh-transactions-api-openapi.yml
  format: yaml
  label: Mesh Transactions API
  slug: mesh-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-transactions-api-openapi.yml
- filename: mesh-transfers-api-openapi.yml
  format: yaml
  label: Mesh Transfers API
  slug: mesh-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/openapi/mesh-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meshconnect.com
  spf: true
hosts:
- cert_expires: Sep 12 06:30:57 2026 GMT
  host: docs.meshconnect.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 06:30:57 2026 GMT
  host: integration-api.meshconnect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mesh, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mesh
provider_slug: mesh
slug: mesh-domain-security
source_filename: mesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.meshconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:30:57 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: integration-api.meshconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:30:57 2026 GMT\n  hsts: null\ndomains:\n- domain: meshconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh/refs/heads/main/security/mesh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Payments
- Digital Assets
- Financial Services
- Wallets
- Exchanges
- Transfers
- Stablecoins
- Embedded Finance
- Fintech
- On-Ramp
- Blockchain
---
