---
api_specs:
- filename: openapi.json
  format: json
  label: Traceloop REST API
  slug: traceloop-rest-api
  spec_type: OpenAPI
  url: https://www.traceloop.com/docs/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: traceloop.com
  spf: true
hosts:
- cert_expires: Oct  1 20:48:08 2026 GMT
  host: www.traceloop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 12:10:43 2026 GMT
  host: api.traceloop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Traceloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traceloop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Traceloop
provider_slug: traceloop
slug: traceloop-domain-security
source_filename: traceloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.traceloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:48:08 2026 GMT\n  hsts: null\n- host: api.traceloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 12:10:43 2026 GMT\n  hsts: null\ndomains:\n- domain: traceloop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traceloop/refs/heads/main/security/traceloop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- LLM Observability
- OpenTelemetry
- AI Monitoring
- Tracing
- Evaluation
- LLM Gateway
- Prompt Management
- Machine Learning
---
