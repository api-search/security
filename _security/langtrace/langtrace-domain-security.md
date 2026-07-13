---
api_specs:
- filename: langtrace-openapi.yml
  format: yaml
  label: Langtrace Trace Ingestion (OTEL)
  slug: trace-ingestion-otel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-openapi.yml
- filename: langtrace-openapi.yml
  format: yaml
  label: Langtrace Projects and API Keys
  slug: projects-api-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-openapi.yml
- filename: langtrace-openapi.yml
  format: yaml
  label: Langtrace Prompt Registry
  slug: prompt-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-openapi.yml
- filename: langtrace-openapi.yml
  format: yaml
  label: Langtrace Trace Retrieval and Metrics
  slug: trace-retrieval
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: langtrace.ai
  spf: true
hosts:
- cert_expires: Aug 16 22:19:29 2026 GMT
  host: www.langtrace.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 06:35:08 2026 GMT
  host: docs.langtrace.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:41:43 2026 GMT
  host: app.langtrace.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Langtrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Langtrace AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Langtrace AI
provider_slug: langtrace
slug: langtrace-domain-security
source_filename: langtrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.langtrace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 22:19:29 2026 GMT\n  hsts: null\n- host: docs.langtrace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:35:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.langtrace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:41:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: langtrace.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/security/langtrace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Observability
- OpenTelemetry
- Tracing
- Open Source
---
