---
api_specs:
- filename: lunary-analytics-api-openapi.yml
  format: yaml
  label: Lunary Analytics API
  slug: lunary-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-analytics-api-openapi.yml
- filename: lunary-auditlogs-api-openapi.yml
  format: yaml
  label: Lunary AuditLogs API
  slug: lunary-auditlogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-auditlogs-api-openapi.yml
- filename: lunary-checklists-api-openapi.yml
  format: yaml
  label: Lunary Checklists API
  slug: lunary-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-checklists-api-openapi.yml
- filename: lunary-datasets-api-openapi.yml
  format: yaml
  label: Lunary Datasets API
  slug: lunary-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-datasets-api-openapi.yml
- filename: lunary-datasetsv2-api-openapi.yml
  format: yaml
  label: Lunary DatasetsV2 API
  slug: lunary-datasetsv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-datasetsv2-api-openapi.yml
- filename: lunary-evals-api-openapi.yml
  format: yaml
  label: Lunary Evals API
  slug: lunary-evals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-evals-api-openapi.yml
- filename: lunary-externalusers-api-openapi.yml
  format: yaml
  label: Lunary ExternalUsers API
  slug: lunary-externalusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-externalusers-api-openapi.yml
- filename: lunary-models-api-openapi.yml
  format: yaml
  label: Lunary Models API
  slug: lunary-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-models-api-openapi.yml
- filename: lunary-playground-api-openapi.yml
  format: yaml
  label: Lunary Playground API
  slug: lunary-playground-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-playground-api-openapi.yml
- filename: lunary-runs-api-openapi.yml
  format: yaml
  label: Lunary Runs API
  slug: lunary-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-runs-api-openapi.yml
- filename: lunary-templates-api-openapi.yml
  format: yaml
  label: Lunary Templates API
  slug: lunary-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-templates-api-openapi.yml
- filename: lunary-testendpoint-api-openapi.yml
  format: yaml
  label: Lunary TestEndpoint API
  slug: lunary-testendpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-testendpoint-api-openapi.yml
- filename: lunary-views-api-openapi.yml
  format: yaml
  label: Lunary Views API
  slug: lunary-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-views-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunary.ai
  spf: false
hosts:
- cert_expires: Sep 24 16:17:16 2026 GMT
  host: lunary.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 03:37:50 2026 GMT
  host: docs.lunary.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:34:59 2026 GMT
  host: api.lunary.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lunary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunary, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Lunary
provider_slug: lunary
slug: lunary-domain-security
source_filename: lunary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lunary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:17:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lunary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:37:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lunary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:34:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lunary.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/security/lunary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Evaluation
- Observability
- Open Source
- LLM
- Tracing
- Prompts
---
