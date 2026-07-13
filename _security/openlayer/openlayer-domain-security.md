---
api_specs:
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Projects API
  slug: openlayer-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Inference Pipelines API
  slug: openlayer-inference-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Data Stream API
  slug: openlayer-data-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Commits and Test Results API
  slug: openlayer-commits-test-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openlayer.com
  spf: true
hosts:
- cert_expires: Sep  4 16:12:47 2026 GMT
  host: www.openlayer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.openlayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openlayer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Openlayer
provider_slug: openlayer
slug: openlayer-domain-security
source_filename: openlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 16:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.openlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: openlayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/security/openlayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Evaluation
- Testing
- Observability
- LLM
- MLOps
---
