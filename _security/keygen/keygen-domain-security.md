---
api_specs:
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Licenses API
  slug: keygen-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Machines / Activation API
  slug: keygen-machines-activation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Policies API
  slug: keygen-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Products API
  slug: keygen-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Users API
  slug: keygen-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Entitlements API
  slug: keygen-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Releases / Distribution API
  slug: keygen-releases-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Artifacts API
  slug: keygen-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Tokens / Auth API
  slug: keygen-tokens-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Webhooks API
  slug: keygen-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Machine Components API
  slug: keygen-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
- filename: keygen-openapi.yml
  format: yaml
  label: Keygen Machine Processes API
  slug: keygen-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/openapi/keygen-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: keygen.sh
  spf: true
hosts:
- cert_expires: Sep  4 12:29:17 2026 GMT
  host: keygen.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keygen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keygen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Keygen
provider_slug: keygen
slug: keygen-domain-security
source_filename: keygen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keygen.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 12:29:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keygen.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keygen/refs/heads/main/security/keygen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software Licensing
- Entitlements
- License Keys
- Machine Activation
- Distribution
- Auto-Update
---
