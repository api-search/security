---
api_specs:
- filename: openapi.json
  format: json
  label: Arize Phoenix REST API
  slug: arize-phoenix-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Arize-ai/phoenix/main/schemas/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arize.com
  spf: true
hosts:
- cert_expires: Aug 15 02:12:54 2026 GMT
  host: arize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 12:54:56 2026 GMT
  host: app.phoenix.arize.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phoenix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arize Phoenix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arize Phoenix
provider_slug: phoenix
slug: phoenix-domain-security
source_filename: phoenix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 02:12:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.phoenix.arize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: arize.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/security/phoenix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LLM Observability
- AI Evaluation
- OpenTelemetry
- Tracing
- LLMOps
- AI Monitoring
- Open Source
- Prompt Engineering
- Datasets
- Experiments
---
