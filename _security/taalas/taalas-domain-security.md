---
api_specs:
- filename: taalas-inference-api-openapi.yml
  format: yaml
  label: Taalas API
  slug: taalas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/openapi/taalas-inference-api-openapi.yml
- filename: taalas-models-api-openapi.yml
  format: yaml
  label: Taalas Models API
  slug: taalas-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/openapi/taalas-models-api-openapi.yml
- filename: taalas-monitoring-api-openapi.yml
  format: yaml
  label: Taalas Monitoring API
  slug: taalas-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/openapi/taalas-monitoring-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: taalas.com
  spf: true
hosts:
- cert_expires: Oct 10 05:21:44 2026 GMT
  host: taalas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 23:59:59 2026 GMT
  host: api.taalas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taalas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taalas, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Taalas
provider_slug: taalas
slug: taalas-domain-security
source_filename: taalas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taalas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 05:21:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.taalas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: taalas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/security/taalas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Inference
- Semiconductors
- AI Accelerator
- Large Language Models
- Llama
- Inference API
- OpenAI-Compatible
- Hardware
- Deep Tech
---
