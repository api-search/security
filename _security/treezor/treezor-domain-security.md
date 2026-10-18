---
api_specs:
- filename: treezor-beneficiaries-api-openapi.yml
  format: yaml
  label: Treezor Beneficiaries API
  slug: treezor-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-beneficiaries-api-openapi.yml
- filename: treezor-cardimages-api-openapi.yml
  format: yaml
  label: Treezor Cardimages API
  slug: treezor-cardimages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-cardimages-api-openapi.yml
- filename: treezor-cards-api-openapi.yml
  format: yaml
  label: Treezor Cards API
  slug: treezor-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-cards-api-openapi.yml
- filename: treezor-core-connect-api-openapi.yml
  format: yaml
  label: Treezor Core Connect API
  slug: treezor-core-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-core-connect-api-openapi.yml
- filename: treezor-customization-api-openapi.yml
  format: yaml
  label: Treezor Customization API
  slug: treezor-customization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-customization-api-openapi.yml
- filename: treezor-default-api-openapi.yml
  format: yaml
  label: Treezor [...] API
  slug: treezor-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-default-api-openapi.yml
- filename: treezor-documents-api-openapi.yml
  format: yaml
  label: Treezor Documents API
  slug: treezor-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-documents-api-openapi.yml
- filename: treezor-oauth-api-openapi.yml
  format: yaml
  label: Treezor OAuth API
  slug: treezor-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-oauth-api-openapi.yml
- filename: treezor-retry-api-openapi.yml
  format: yaml
  label: Treezor Retry API
  slug: treezor-retry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-retry-api-openapi.yml
- filename: treezor-simulation-api-openapi.yml
  format: yaml
  label: Treezor Simulation API
  slug: treezor-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-simulation-api-openapi.yml
- filename: treezor-treezor-api-api-openapi.yml
  format: yaml
  label: Treezor Treezor API
  slug: treezor-treezor-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-treezor-api-api-openapi.yml
- filename: treezor-users-api-openapi.yml
  format: yaml
  label: Treezor Users API
  slug: treezor-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-users-api-openapi.yml
- filename: treezor-wallets-api-openapi.yml
  format: yaml
  label: Treezor Wallets API
  slug: treezor-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/treezor-wallets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: treezor.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.treezor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Treezor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treezor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Treezor
provider_slug: treezor
slug: treezor-domain-security
source_filename: treezor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treezor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: treezor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/security/treezor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Payments
- Banking as a Service
- Europe
---
