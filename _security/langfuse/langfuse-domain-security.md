---
api_specs:
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Tracing API
  slug: langfuse-tracing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Observations API
  slug: langfuse-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Metrics API
  slug: langfuse-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Prompt Management API
  slug: langfuse-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Datasets API
  slug: langfuse-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Evaluations API
  slug: langfuse-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Scores API
  slug: langfuse-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Organizations & Projects API
  slug: langfuse-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Instance Management API
  slug: langfuse-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: langfuse.com
  spf: true
hosts:
- cert_expires: Aug 12 08:48:37 2026 GMT
  host: langfuse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: cloud.langfuse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Langfuse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Langfuse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Langfuse
provider_slug: langfuse
slug: langfuse-domain-security
source_filename: langfuse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: langfuse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 08:48:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.langfuse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: langfuse.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/security/langfuse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- LLM
- Observability
- Open Source
- Evaluations
---
