---
api_specs:
- filename: opik-rest-api-openapi.yml
  format: yaml
  label: Opik REST API
  slug: opik-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opik/refs/heads/main/openapi/opik-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: comet.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.comet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Opik
provider_slug: opik
slug: opik-domain-security
source_filename: opik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: comet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opik/refs/heads/main/security/opik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LLM
- Evaluation
- Observability
- Tracing
- Open Source
- LLMOps
- RAG
- AI
- Machine Learning
- Monitoring
---
