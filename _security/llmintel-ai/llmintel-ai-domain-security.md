---
api_specs:
- filename: llmintel-ai-compare-api-openapi.yml
  format: yaml
  label: llmintel-ai Compare API
  slug: llmintel-ai-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-compare-api-openapi.yml
- filename: llmintel-ai-events-api-openapi.yml
  format: yaml
  label: llmintel-ai Events API
  slug: llmintel-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-events-api-openapi.yml
- filename: llmintel-ai-models-api-openapi.yml
  format: yaml
  label: llmintel-ai Models API
  slug: llmintel-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-models-api-openapi.yml
- filename: llmintel-ai-status-api-openapi.yml
  format: yaml
  label: llmintel-ai Status API
  slug: llmintel-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-status-api-openapi.yml
- filename: llmintel-ai-telemetry-api-openapi.yml
  format: yaml
  label: llmintel-ai Telemetry API
  slug: llmintel-ai-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-telemetry-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: llmintel.ai
  spf: false
hosts:
- cert_expires: Nov 28 21:03:12 2026 GMT
  host: llmintel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmintel Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for llmintel-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: llmintel-ai
provider_slug: llmintel-ai
slug: llmintel-ai-domain-security
source_filename: llmintel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmintel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 21:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: llmintel.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/llmintel-ai/security/llmintel-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Cost
- Observability
- Telemetry
- GenAI
---
