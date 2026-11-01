---
api_specs:
- filename: asoskill-com-authentication-api-openapi.yml
  format: yaml
  label: asoskill-com Authentication API
  slug: asoskill-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-authentication-api-openapi.yml
- filename: asoskill-com-billing-api-openapi.yml
  format: yaml
  label: asoskill-com Billing API
  slug: asoskill-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-billing-api-openapi.yml
- filename: asoskill-com-credits-api-openapi.yml
  format: yaml
  label: asoskill-com Credits API
  slug: asoskill-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-credits-api-openapi.yml
- filename: asoskill-com-data-api-openapi.yml
  format: yaml
  label: asoskill-com Data API
  slug: asoskill-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-data-api-openapi.yml
- filename: asoskill-com-mcp-api-openapi.yml
  format: yaml
  label: asoskill-com MCP API
  slug: asoskill-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-mcp-api-openapi.yml
- filename: asoskill-com-operations-api-openapi.yml
  format: yaml
  label: asoskill-com Operations API
  slug: asoskill-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-operations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asoskill.com
  spf: false
hosts:
- cert_expires: Dec 15 17:37:58 2026 GMT
  host: asoskill.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asoskill Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for asoskill-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: asoskill-com
provider_slug: asoskill-com
slug: asoskill-com-domain-security
source_filename: asoskill-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asoskill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 17:37:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: asoskill.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/asoskill-com/security/asoskill-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- ASO
- AppStore
- API
- Data
---
