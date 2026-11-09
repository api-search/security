---
api_specs:
- filename: mesh-assets-api-openapi.yml
  format: yaml
  label: Mesh Assets API
  slug: mesh-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-assets-api-openapi.yml
- filename: mesh-balance-api-openapi.yml
  format: yaml
  label: Mesh Balance API
  slug: mesh-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-balance-api-openapi.yml
- filename: mesh-brokeraccountdetail-api-openapi.yml
  format: yaml
  label: Mesh BrokerAccountDetail API
  slug: mesh-brokeraccountdetail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-brokeraccountdetail-api-openapi.yml
- filename: mesh-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Managed Account Authentication API
  slug: mesh-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-managed-account-authentication-api-openapi.yml
- filename: mesh-managed-transfers-api-openapi.yml
  format: yaml
  label: Mesh Managed Transfers API
  slug: mesh-managed-transfers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-managed-transfers-api-openapi.yml
- filename: mesh-portfolio-api-openapi.yml
  format: yaml
  label: Mesh Portfolio API
  slug: mesh-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-portfolio-api-openapi.yml
- filename: mesh-self-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Self Managed Account Authentication API
  slug: mesh-self-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-self-managed-account-authentication-api-openapi.yml
- filename: mesh-transactions-api-openapi.yml
  format: yaml
  label: Mesh Transactions API
  slug: mesh-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-transactions-api-openapi.yml
- filename: mesh-transfers-api-openapi.yml
  format: yaml
  label: Mesh Transfers API
  slug: mesh-transfers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-transfers-api-openapi.yml
- filename: mesh-blockchainquery-api-openapi.yml
  format: yaml
  label: Mesh Blockchain Query API
  slug: mesh-blockchainquery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-blockchainquery-api-openapi.yml
- filename: mesh-cataloggassponsorship-api-openapi.yml
  format: yaml
  label: Mesh Catalog Gas Sponsorship API
  slug: mesh-cataloggassponsorship-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-cataloggassponsorship-api-openapi.yml
- filename: mesh-catalogsubscription-api-openapi.yml
  format: yaml
  label: Mesh Catalog Subscription API
  slug: mesh-catalogsubscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-catalogsubscription-api-openapi.yml
- filename: mesh-headless-bridging-api-openapi.yml
  format: yaml
  label: Mesh Headless Bridging API
  slug: mesh-headless-bridging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-headless-bridging-api-openapi.yml
- filename: mesh-integrations-account-information-api-openapi.yml
  format: yaml
  label: Mesh Integrations account information API
  slug: mesh-integrations-account-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-integrations-account-information-api-openapi.yml
- filename: mesh-rampkyc-api-openapi.yml
  format: yaml
  label: Mesh Ramp Kyc API
  slug: mesh-rampkyc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-rampkyc-api-openapi.yml
- filename: mesh-ramppayment-api-openapi.yml
  format: yaml
  label: Mesh Ramp Payment API
  slug: mesh-ramppayment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-ramppayment-api-openapi.yml
- filename: mesh-rampsession-api-openapi.yml
  format: yaml
  label: Mesh Ramp Session API
  slug: mesh-rampsession-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-rampsession-api-openapi.yml
- filename: mesh-tokennetworkpairs-api-openapi.yml
  format: yaml
  label: Mesh Token Network Pairs API
  slug: mesh-tokennetworkpairs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-tokennetworkpairs-api-openapi.yml
- filename: mesh-wallets-api-openapi.yml
  format: yaml
  label: Mesh Wallets API
  slug: mesh-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mesh/openapi/mesh-wallets-api-openapi.yml
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
hosts_probed: 2
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
source_yaml_url: https://artifacts.apis.io/mesh/security/mesh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Payments
- Digital Assets
- Financial Services
- Wallets
- Exchange
- Transfers
- Stablecoins
- Embedded Finance
- Fintech
- On-Ramp
- Blockchain
---
