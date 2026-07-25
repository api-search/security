---
api_specs:
- filename: dfns-approvals-api-openapi.yml
  format: yaml
  label: Dfns Approvals API
  slug: dfns-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-approvals-api-openapi.yml
- filename: dfns-auth-api-openapi.yml
  format: yaml
  label: Dfns Auth API
  slug: dfns-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-auth-api-openapi.yml
- filename: dfns-keys-api-openapi.yml
  format: yaml
  label: Dfns Keys API
  slug: dfns-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-keys-api-openapi.yml
- filename: dfns-networks-api-openapi.yml
  format: yaml
  label: Dfns Networks API
  slug: dfns-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-networks-api-openapi.yml
- filename: dfns-permissions-api-openapi.yml
  format: yaml
  label: Dfns Permissions API
  slug: dfns-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-permissions-api-openapi.yml
- filename: dfns-policies-api-openapi.yml
  format: yaml
  label: Dfns Policies API
  slug: dfns-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-policies-api-openapi.yml
- filename: dfns-serviceaccounts-api-openapi.yml
  format: yaml
  label: Dfns ServiceAccounts API
  slug: dfns-serviceaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-serviceaccounts-api-openapi.yml
- filename: dfns-signatures-api-openapi.yml
  format: yaml
  label: Dfns Signatures API
  slug: dfns-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-signatures-api-openapi.yml
- filename: dfns-transactions-api-openapi.yml
  format: yaml
  label: Dfns Transactions API
  slug: dfns-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-transactions-api-openapi.yml
- filename: dfns-transfers-api-openapi.yml
  format: yaml
  label: Dfns Transfers API
  slug: dfns-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-transfers-api-openapi.yml
- filename: dfns-wallets-api-openapi.yml
  format: yaml
  label: Dfns Wallets API
  slug: dfns-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-wallets-api-openapi.yml
- filename: dfns-webhooks-api-openapi.yml
  format: yaml
  label: Dfns Webhooks API
  slug: dfns-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/openapi/dfns-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dfns.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dfns.io
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.dfns.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:55:59 2026 GMT
  host: docs.dfns.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: api.dfns.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dfns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dfns, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dfns
provider_slug: dfns
slug: dfns-domain-security
source_filename: dfns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dfns.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dfns.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:55:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dfns.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dfns.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dfns.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dfns/refs/heads/main/security/dfns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Wallets
- MPC
- Key Management
- Digital Assets
- Web3
- Non-Custodial
---
