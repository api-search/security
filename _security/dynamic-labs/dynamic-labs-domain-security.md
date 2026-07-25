---
api_specs:
- filename: dynamic-labs-allowlists-api-openapi.yml
  format: yaml
  label: Dynamic Allowlists API
  slug: dynamic-labs-allowlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-allowlists-api-openapi.yml
- filename: dynamic-labs-analytics-api-openapi.yml
  format: yaml
  label: Dynamic Analytics API
  slug: dynamic-labs-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-analytics-api-openapi.yml
- filename: dynamic-labs-api-tokens-api-openapi.yml
  format: yaml
  label: Dynamic API Tokens API
  slug: dynamic-labs-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-api-tokens-api-openapi.yml
- filename: dynamic-labs-embedded-wallets-api-openapi.yml
  format: yaml
  label: Dynamic Embedded Wallets API
  slug: dynamic-labs-embedded-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-embedded-wallets-api-openapi.yml
- filename: dynamic-labs-environments-api-openapi.yml
  format: yaml
  label: Dynamic Environments API
  slug: dynamic-labs-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-environments-api-openapi.yml
- filename: dynamic-labs-exports-api-openapi.yml
  format: yaml
  label: Dynamic Exports API
  slug: dynamic-labs-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-exports-api-openapi.yml
- filename: dynamic-labs-jwks-api-openapi.yml
  format: yaml
  label: Dynamic JWKS API
  slug: dynamic-labs-jwks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-jwks-api-openapi.yml
- filename: dynamic-labs-users-api-openapi.yml
  format: yaml
  label: Dynamic Users API
  slug: dynamic-labs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-users-api-openapi.yml
- filename: dynamic-labs-wallets-api-openapi.yml
  format: yaml
  label: Dynamic Wallets API
  slug: dynamic-labs-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-wallets-api-openapi.yml
- filename: dynamic-labs-webhooks-api-openapi.yml
  format: yaml
  label: Dynamic Webhooks API
  slug: dynamic-labs-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dynamic.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dynamicauth.com
  spf: true
hosts:
- cert_expires: Aug 14 10:18:41 2026 GMT
  host: www.dynamic.xyz
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 21:16:47 2026 GMT
  host: app.dynamicauth.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 15:30:47 2026 GMT
  host: app.dynamic.xyz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dynamic Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dynamic
provider_slug: dynamic-labs
slug: dynamic-labs-domain-security
source_filename: dynamic-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dynamic.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 10:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: app.dynamicauth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:16:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.dynamic.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 15:30:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: dynamic.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dynamicauth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/security/dynamic-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Authentication
- Embedded Wallets
- Wallets
- MPC
- Onboarding
- Crypto
---
