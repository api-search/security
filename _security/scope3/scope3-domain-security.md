---
api_specs:
- filename: scope3-buyer-openapi-original.yml
  format: yaml
  label: Scope3 Interchange Buyer API
  slug: scope3-interchange-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/_original/scope3-buyer-openapi-original.yml
- filename: scope3-storefront-openapi-original.yml
  format: yaml
  label: Scope3 Interchange Storefront API
  slug: scope3-interchange-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/_original/scope3-storefront-openapi-original.yml
- filename: scope3-ai-impact-measurement-api-openapi.yml
  format: yaml
  label: Scope3 AI Impact Measurement API
  slug: scope3-ai-impact-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-ai-impact-measurement-api-openapi.yml
- filename: scope3-benchmarks-api-openapi.yml
  format: yaml
  label: Scope3 Benchmarks API
  slug: scope3-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-benchmarks-api-openapi.yml
- filename: scope3-creative-api-openapi.yml
  format: yaml
  label: Scope3 Creative API
  slug: scope3-creative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-creative-api-openapi.yml
- filename: scope3-data-api-openapi.yml
  format: yaml
  label: Scope3 Data API
  slug: scope3-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-data-api-openapi.yml
- filename: scope3-gpu-api-openapi.yml
  format: yaml
  label: Scope3 Gpu API
  slug: scope3-gpu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-gpu-api-openapi.yml
- filename: scope3-impact-api-openapi.yml
  format: yaml
  label: Scope3 Impact API
  slug: scope3-impact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-impact-api-openapi.yml
- filename: scope3-measure-api-openapi.yml
  format: yaml
  label: Scope3 Measure API
  slug: scope3-measure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-measure-api-openapi.yml
- filename: scope3-model-api-openapi.yml
  format: yaml
  label: Scope3 Model API
  slug: scope3-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-model-api-openapi.yml
- filename: scope3-node-api-openapi.yml
  format: yaml
  label: Scope3 Node API
  slug: scope3-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-node-api-openapi.yml
- filename: scope3-reload-api-openapi.yml
  format: yaml
  label: Scope3 Reload API
  slug: scope3-reload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-reload-api-openapi.yml
- filename: scope3-saved-lists-api-openapi.yml
  format: yaml
  label: Scope3 Saved Lists API
  slug: scope3-saved-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-saved-lists-api-openapi.yml
- filename: scope3-segment-api-openapi.yml
  format: yaml
  label: Scope3 Segment API
  slug: scope3-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-segment-api-openapi.yml
- filename: scope3-signals-api-openapi.yml
  format: yaml
  label: Scope3 Signals API
  slug: scope3-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-signals-api-openapi.yml
- filename: scope3-status-api-openapi.yml
  format: yaml
  label: Scope3 Status API
  slug: scope3-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scope3.com
  spf: true
hosts:
- cert_expires: Sep 30 21:56:56 2026 GMT
  host: scope3.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:56:51 2026 GMT
  host: docs.scope3.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 19:53:05 2026 GMT
  host: api.agentic.scope3.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scope3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scope3, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Scope3
provider_slug: scope3
slug: scope3-domain-security
source_filename: scope3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scope3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:56:56 2026 GMT\n  hsts: false\n- host: docs.scope3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:56:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.agentic.scope3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 19:53:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scope3.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/security/scope3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Advertising
- Carbon Emissions
- Sustainability
- AdTech
- Measurement
- Artificial Intelligence
- Agentic
- AdCP
- MCP
- Programmatic
- Media Buying
- Publishing
---
