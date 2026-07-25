---
api_specs:
- filename: mesh-connect-assets-api-openapi.yml
  format: yaml
  label: Mesh Connect Assets API
  slug: mesh-connect-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-assets-api-openapi.yml
- filename: mesh-connect-auth-token-api-openapi.yml
  format: yaml
  label: Mesh Connect Auth token API
  slug: mesh-connect-auth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-auth-token-api-openapi.yml
- filename: mesh-connect-balance-api-openapi.yml
  format: yaml
  label: Mesh Connect Balance API
  slug: mesh-connect-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-balance-api-openapi.yml
- filename: mesh-connect-brokeraccountdetail-api-openapi.yml
  format: yaml
  label: Mesh Connect BrokerAccountDetail API
  slug: mesh-connect-brokeraccountdetail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-brokeraccountdetail-api-openapi.yml
- filename: mesh-connect-main-clients-api-openapi.yml
  format: yaml
  label: Mesh Connect Main Clients API
  slug: mesh-connect-main-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-main-clients-api-openapi.yml
- filename: mesh-connect-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Connect Managed Account Authentication API
  slug: mesh-connect-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-managed-account-authentication-api-openapi.yml
- filename: mesh-connect-managed-transfers-api-openapi.yml
  format: yaml
  label: Mesh Connect Managed Transfers API
  slug: mesh-connect-managed-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-managed-transfers-api-openapi.yml
- filename: mesh-connect-portfolio-api-openapi.yml
  format: yaml
  label: Mesh Connect Portfolio API
  slug: mesh-connect-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-portfolio-api-openapi.yml
- filename: mesh-connect-registered-clients-api-openapi.yml
  format: yaml
  label: Mesh Connect Registered Clients API
  slug: mesh-connect-registered-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-registered-clients-api-openapi.yml
- filename: mesh-connect-self-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Connect Self Managed Account Authentication API
  slug: mesh-connect-self-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-self-managed-account-authentication-api-openapi.yml
- filename: mesh-connect-transactions-api-openapi.yml
  format: yaml
  label: Mesh Connect Transactions API
  slug: mesh-connect-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-transactions-api-openapi.yml
- filename: mesh-connect-transfers-api-openapi.yml
  format: yaml
  label: Mesh Connect Transfers API
  slug: mesh-connect-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meshconnect.com
  spf: true
hosts:
- cert_expires: Oct 15 02:09:24 2026 GMT
  host: www.meshconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: admin-api.meshconnect.com
  hsts: null
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
name: Mesh Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mesh Connect, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mesh Connect
provider_slug: mesh-connect
slug: mesh-connect-domain-security
source_filename: mesh-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meshconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:09:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: admin-api.meshconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n- host: integration-api.meshconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:30:57 2026 GMT\n  hsts: null\ndomains:\n- domain: meshconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/security/mesh-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Infrastructure
- Crypto Payments
- Digital Assets
- Wallets
- Exchanges
- Embedded Finance
- Stablecoins
- Payments
---
