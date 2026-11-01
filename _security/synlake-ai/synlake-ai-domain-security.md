---
api_specs:
- filename: synlake-ai-auth-api-openapi.yml
  format: yaml
  label: synlake-ai Auth API
  slug: synlake-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-auth-api-openapi.yml
- filename: synlake-ai-billing-api-openapi.yml
  format: yaml
  label: synlake-ai Billing API
  slug: synlake-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-billing-api-openapi.yml
- filename: synlake-ai-catalog-api-openapi.yml
  format: yaml
  label: synlake-ai Catalog API
  slug: synlake-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-catalog-api-openapi.yml
- filename: synlake-ai-execution-api-openapi.yml
  format: yaml
  label: synlake-ai Execution API
  slug: synlake-ai-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-execution-api-openapi.yml
- filename: synlake-ai-infrastructure-api-openapi.yml
  format: yaml
  label: synlake-ai Infrastructure API
  slug: synlake-ai-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-infrastructure-api-openapi.yml
- filename: synlake-ai-system-api-openapi.yml
  format: yaml
  label: synlake-ai System API
  slug: synlake-ai-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-system-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: synlake.ai
  spf: true
hosts:
- cert_expires: Nov 29 06:36:40 2026 GMT
  host: synlake.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synlake Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for synlake-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: synlake-ai
provider_slug: synlake-ai
slug: synlake-ai-domain-security
source_filename: synlake-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synlake.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 06:36:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: synlake.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/synlake-ai/security/synlake-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Infrastructure
- AI Agents
- Cloud
- Terraform
- API
---
