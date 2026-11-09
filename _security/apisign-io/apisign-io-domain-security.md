---
api_specs:
- filename: apisign-io-api-keys-api-openapi.yml
  format: yaml
  label: APISign API Keys API
  slug: apisign-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-api-keys-api-openapi.yml
- filename: apisign-io-contracts-api-openapi.yml
  format: yaml
  label: APISign Contracts API
  slug: apisign-io-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-contracts-api-openapi.yml
- filename: apisign-io-health-api-openapi.yml
  format: yaml
  label: APISign Health API
  slug: apisign-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-health-api-openapi.yml
- filename: apisign-io-organization-api-openapi.yml
  format: yaml
  label: APISign Organization API
  slug: apisign-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-organization-api-openapi.yml
- filename: apisign-io-templates-api-openapi.yml
  format: yaml
  label: APISign Templates API
  slug: apisign-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-templates-api-openapi.yml
- filename: apisign-io-webhooks-api-openapi.yml
  format: yaml
  label: APISign Webhooks API
  slug: apisign-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apisign.io
  spf: true
hosts:
- cert_expires: Dec  2 23:49:54 2026 GMT
  host: apisign.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apisign Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APISign, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APISign
provider_slug: apisign-io
slug: apisign-io-domain-security
source_filename: apisign-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apisign.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:49:54 2026 GMT\n  hsts: false\ndomains:\n- domain: apisign.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/apisign-io/security/apisign-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Signature
- Artificial Intelligence
- MCP
- Contracts
- Developer Platform
---
