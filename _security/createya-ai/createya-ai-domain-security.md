---
api_specs:
- filename: createya-ai-balance-api-openapi.yml
  format: yaml
  label: Createya Balance API
  slug: createya-ai-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-balance-api-openapi.yml
- filename: createya-ai-healthz-api-openapi.yml
  format: yaml
  label: Createya Healthz API
  slug: createya-ai-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-healthz-api-openapi.yml
- filename: createya-ai-mcp-api-openapi.yml
  format: yaml
  label: Createya MCP API
  slug: createya-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-mcp-api-openapi.yml
- filename: createya-ai-models-api-openapi.yml
  format: yaml
  label: Createya Models API
  slug: createya-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-models-api-openapi.yml
- filename: createya-ai-run-api-openapi.yml
  format: yaml
  label: Createya Run API
  slug: createya-ai-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-run-api-openapi.yml
- filename: createya-ai-runs-api-openapi.yml
  format: yaml
  label: Createya Runs API
  slug: createya-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-runs-api-openapi.yml
- filename: createya-ai-uploads-api-openapi.yml
  format: yaml
  label: Createya Uploads API
  slug: createya-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-uploads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: createya.ai
  spf: true
hosts:
- cert_expires: Dec  5 02:13:45 2026 GMT
  host: createya.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Createya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Createya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Createya
provider_slug: createya-ai
slug: createya-ai-domain-security
source_filename: createya-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: createya.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 02:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: createya.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/createya-ai/security/createya-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Audio Generation
- Model Aggregator
- MCP
---
