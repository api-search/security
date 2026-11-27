---
api_specs:
- filename: odei-ai-agent-access-api-openapi.yml
  format: yaml
  label: ODEI Agent Access API
  slug: odei-ai-agent-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-agent-access-api-openapi.yml
- filename: odei-ai-bidwall-api-openapi.yml
  format: yaml
  label: ODEI Bidwall API
  slug: odei-ai-bidwall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-bidwall-api-openapi.yml
- filename: odei-ai-blink-api-openapi.yml
  format: yaml
  label: ODEI Blink API
  slug: odei-ai-blink-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-blink-api-openapi.yml
- filename: odei-ai-context-api-openapi.yml
  format: yaml
  label: ODEI Context API
  slug: odei-ai-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-context-api-openapi.yml
- filename: odei-ai-health-api-openapi.yml
  format: yaml
  label: ODEI Health API
  slug: odei-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-health-api-openapi.yml
- filename: odei-ai-intake-api-openapi.yml
  format: yaml
  label: ODEI Intake API
  slug: odei-ai-intake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-intake-api-openapi.yml
- filename: odei-ai-integrations-api-openapi.yml
  format: yaml
  label: ODEI Integrations API
  slug: odei-ai-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-integrations-api-openapi.yml
- filename: odei-ai-mcp-api-openapi.yml
  format: yaml
  label: ODEI MCP API
  slug: odei-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-mcp-api-openapi.yml
- filename: odei-ai-openapi-json-api-openapi.yml
  format: yaml
  label: ODEI Openapi.json API
  slug: odei-ai-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-openapi-json-api-openapi.yml
- filename: odei-ai-openapi-v2-yaml-api-openapi.yml
  format: yaml
  label: ODEI Openapi V2.yaml API
  slug: odei-ai-openapi-v2-yaml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-openapi-v2-yaml-api-openapi.yml
- filename: odei-ai-revenue-api-openapi.yml
  format: yaml
  label: ODEI Revenue API
  slug: odei-ai-revenue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-revenue-api-openapi.yml
- filename: odei-ai-site-metrics-api-openapi.yml
  format: yaml
  label: ODEI Site Metrics API
  slug: odei-ai-site-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-site-metrics-api-openapi.yml
- filename: odei-ai-token-api-openapi.yml
  format: yaml
  label: ODEI Token API
  slug: odei-ai-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-token-api-openapi.yml
- filename: odei-ai-well-known-api-openapi.yml
  format: yaml
  label: ODEI .well Known API
  slug: odei-ai-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-well-known-api-openapi.yml
- filename: odei-ai-worldmodel-api-openapi.yml
  format: yaml
  label: ODEI Worldmodel API
  slug: odei-ai-worldmodel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odei-ai/openapi/odei-ai-worldmodel-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: odei.ai
  spf: true
hosts:
- cert_expires: Feb  3 22:35:23 2027 GMT
  host: odei.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ODEI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ODEI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ODEI
provider_slug: odei-ai
slug: odei-ai-domain-security
source_filename: odei-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: odei.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 22:35:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: odei.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/odei-ai/security/odei-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Personal Data
- Platform
- Cloud
- Desktop
---
