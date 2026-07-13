---
api_specs:
- filename: athina-openapi.yml
  format: yaml
  label: Athina Logging & Inferences API
  slug: athina-logging-inferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
- filename: athina-openapi.yml
  format: yaml
  label: Athina Datasets API
  slug: athina-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
- filename: athina-openapi.yml
  format: yaml
  label: Athina Evaluations API
  slug: athina-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
- filename: athina-openapi.yml
  format: yaml
  label: Athina Prompts API
  slug: athina-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
- filename: athina-openapi.yml
  format: yaml
  label: Athina Experiments API
  slug: athina-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: athina.ai
  spf: true
hosts:
- cert_expires: Aug 21 19:00:16 2026 GMT
  host: www.athina.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 14:17:42 2026 GMT
  host: docs.athina.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 04:00:34 2026 GMT
  host: api.athina.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Athina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Athina AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Athina AI
provider_slug: athina
slug: athina-domain-security
source_filename: athina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.athina.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.athina.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:17:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.athina.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:00:34 2026 GMT\n  hsts: null\ndomains:\n- domain: athina.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/security/athina-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- LLM
- Observability
- Evaluation
- Monitoring
---
