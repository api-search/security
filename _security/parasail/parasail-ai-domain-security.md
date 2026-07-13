---
api_specs:
- filename: parasail-inference-api-openapi.yml
  format: yaml
  label: Parasail Inference API
  slug: parasail-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail/refs/heads/main/openapi/parasail-inference-api-openapi.yml
- filename: parasail-batch-api-openapi.yml
  format: yaml
  label: Parasail Batch API
  slug: parasail-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail/refs/heads/main/openapi/parasail-batch-api-openapi.yml
- filename: parasail-dedicated-api-openapi.yml
  format: yaml
  label: Parasail Dedicated Deployments API
  slug: parasail-dedicated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail/refs/heads/main/openapi/parasail-dedicated-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parasail.io
  spf: true
hosts:
- cert_expires: Sep 20 20:42:49 2026 GMT
  host: parasail.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 10:27:14 2026 GMT
  host: docs.parasail.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 13:48:35 2026 GMT
  host: api.parasail.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parasail Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parasail, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parasail
provider_slug: parasail
slug: parasail-ai-domain-security
source_filename: parasail-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parasail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:42:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.parasail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 10:27:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.parasail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:48:35 2026 GMT\n  hsts: null\ndomains:\n- domain: parasail.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parasail/refs/heads/main/security/parasail-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- GPU
- Inference
- Large Language Models
- Open Source Models
- Hugging Face
- Batch
- Embeddings
- Tokenmaxxing
- Supercloud
---
