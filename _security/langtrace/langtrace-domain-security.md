---
api_specs:
- filename: langtrace-projects-api-openapi.yml
  format: yaml
  label: Langtrace AI Projects API
  slug: langtrace-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-projects-api-openapi.yml
- filename: langtrace-prompt-registry-api-openapi.yml
  format: yaml
  label: Langtrace AI Prompt Registry API
  slug: langtrace-prompt-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-prompt-registry-api-openapi.yml
- filename: langtrace-traces-api-openapi.yml
  format: yaml
  label: Langtrace AI Traces API
  slug: langtrace-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-traces-api-openapi.yml
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
