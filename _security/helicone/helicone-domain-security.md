---
api_specs:
- filename: swagger.json
  format: json
  label: Helicone
  slug: helicone
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: ai-gateway.openapi.json
  format: json
  label: Helicone AI Gateway API
  slug: ai-gateway-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/ai-gateway.openapi.json
- filename: swagger.json
  format: json
  label: Helicone Request API
  slug: request-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Prompt API
  slug: prompt-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Experiment API
  slug: experiment-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Evals API
  slug: evals-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Session API
  slug: session-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone User API
  slug: user-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Webhook API
  slug: webhook-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Model Registry API
  slug: model-registry-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Trace API
  slug: trace-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Dashboard API
  slug: dashboard-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Property API
  slug: property-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helicone.ai
  spf: true
hosts:
- cert_expires: Sep 14 20:19:01 2026 GMT
  host: us.helicone.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 13:04:00 2026 GMT
  host: www.helicone.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 19:59:29 2026 GMT
  host: docs.helicone.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helicone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helicone, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Helicone
provider_slug: helicone
slug: helicone-domain-security
source_filename: helicone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: us.helicone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.helicone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.helicone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:59:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: helicone.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helicone/refs/heads/main/security/helicone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Gateways
- AI Monitoring
- Gateways
- LLM Observability
- LLM Routing
- Prompt Management
---
