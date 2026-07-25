---
api_specs:
- filename: tesser-accounts-api-openapi.yml
  format: yaml
  label: Tesser Accounts API
  slug: tesser-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-accounts-api-openapi.yml
- filename: tesser-admin-api-openapi.yml
  format: yaml
  label: Tesser Admin API
  slug: tesser-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-admin-api-openapi.yml
- filename: tesser-api-keys-api-openapi.yml
  format: yaml
  label: Tesser API Keys API
  slug: tesser-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-api-keys-api-openapi.yml
- filename: tesser-counterparties-api-openapi.yml
  format: yaml
  label: Tesser Counterparties API
  slug: tesser-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-counterparties-api-openapi.yml
- filename: tesser-currencies-api-openapi.yml
  format: yaml
  label: Tesser Currencies API
  slug: tesser-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-currencies-api-openapi.yml
- filename: tesser-health-api-openapi.yml
  format: yaml
  label: Tesser health API
  slug: tesser-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-health-api-openapi.yml
- filename: tesser-mcp-api-openapi.yml
  format: yaml
  label: Tesser MCP API
  slug: tesser-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-mcp-api-openapi.yml
- filename: tesser-networks-api-openapi.yml
  format: yaml
  label: Tesser Networks API
  slug: tesser-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-networks-api-openapi.yml
- filename: tesser-organizations-api-openapi.yml
  format: yaml
  label: Tesser Organizations API
  slug: tesser-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-organizations-api-openapi.yml
- filename: tesser-payments-api-openapi.yml
  format: yaml
  label: Tesser Payments API
  slug: tesser-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-payments-api-openapi.yml
- filename: tesser-tenants-api-openapi.yml
  format: yaml
  label: Tesser Tenants API
  slug: tesser-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-tenants-api-openapi.yml
- filename: tesser-treasury-api-openapi.yml
  format: yaml
  label: Tesser Treasury API
  slug: tesser-treasury-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-treasury-api-openapi.yml
- filename: tesser-users-api-openapi.yml
  format: yaml
  label: Tesser Users API
  slug: tesser-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-users-api-openapi.yml
- filename: tesser-webhooks-api-openapi.yml
  format: yaml
  label: Tesser webhooks API
  slug: tesser-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tesser.xyz
  spf: true
hosts:
- cert_expires: Oct  1 09:16:07 2026 GMT
  host: tesser.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 01:28:47 2026 GMT
  host: docs.tesser.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:41:20 2026 GMT
  host: api.tesser.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesser, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tesser
provider_slug: tesser
slug: tesser-domain-security
source_filename: tesser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tesser.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tesser.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:28:47 2026 GMT\n  hsts: false\n- host: api.tesser.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:41:20 2026 GMT\n  hsts: null\ndomains:\n- domain: tesser.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/security/tesser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Stablecoins
- Cross-Border Payments
- Fintech
- Treasury
- Banking
- Blockchain
- Compliance
- MCP
- Developer Platform
---
