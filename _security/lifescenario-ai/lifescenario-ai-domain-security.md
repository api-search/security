---
api_specs:
- filename: lifescenario-ai-health-api-openapi.yml
  format: yaml
  label: Life Scenario Health API
  slug: lifescenario-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lifescenario-ai/openapi/lifescenario-ai-health-api-openapi.yml
- filename: lifescenario-ai-mcp-api-openapi.yml
  format: yaml
  label: Life Scenario MCP API
  slug: lifescenario-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lifescenario-ai/openapi/lifescenario-ai-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lifescenario.ai
  spf: true
hosts:
- cert_expires: Jan  6 06:42:01 2027 GMT
  host: lifescenario.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Life Scenario Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Life Scenario, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Life Scenario
provider_slug: lifescenario-ai
slug: lifescenario-ai-domain-security
source_filename: lifescenario-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lifescenario.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 06:42:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lifescenario.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lifescenario-ai/security/lifescenario-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Children
- Social Emotional Learning
- Gamified
- Artificial Intelligence
---
