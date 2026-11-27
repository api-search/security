---
api_specs:
- filename: gvnr-dev-account-api-openapi.yml
  format: yaml
  label: Gvnr Account API
  slug: gvnr-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-account-api-openapi.yml
- filename: gvnr-dev-approval-api-openapi.yml
  format: yaml
  label: Gvnr Approval API
  slug: gvnr-dev-approval-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-approval-api-openapi.yml
- filename: gvnr-dev-approve-api-openapi.yml
  format: yaml
  label: Gvnr Approve API
  slug: gvnr-dev-approve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-approve-api-openapi.yml
- filename: gvnr-dev-budget-api-openapi.yml
  format: yaml
  label: Gvnr Budget API
  slug: gvnr-dev-budget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-budget-api-openapi.yml
- filename: gvnr-dev-idempotency-api-openapi.yml
  format: yaml
  label: Gvnr Idempotency API
  slug: gvnr-dev-idempotency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-idempotency-api-openapi.yml
- filename: gvnr-dev-mcp-api-openapi.yml
  format: yaml
  label: Gvnr MCP API
  slug: gvnr-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-mcp-api-openapi.yml
- filename: gvnr-dev-packs-api-openapi.yml
  format: yaml
  label: Gvnr Packs API
  slug: gvnr-dev-packs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-packs-api-openapi.yml
- filename: gvnr-dev-rate-api-openapi.yml
  format: yaml
  label: Gvnr Rate API
  slug: gvnr-dev-rate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-rate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gvnr.dev
  spf: true
hosts:
- cert_expires: Dec 12 15:29:30 2026 GMT
  host: gvnr.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gvnr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gvnr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gvnr
provider_slug: gvnr-dev
slug: gvnr-dev-domain-security
source_filename: gvnr-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gvnr.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gvnr.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gvnr-dev/security/gvnr-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Budgets
- SpendControl
- MCP
- Finance
---
