---
api_specs:
- filename: lamini-classify-api-openapi.yml
  format: yaml
  label: Lamini Classify API
  slug: lamini-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-classify-api-openapi.yml
- filename: lamini-embeddings-api-openapi.yml
  format: yaml
  label: Lamini Embeddings API
  slug: lamini-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-embeddings-api-openapi.yml
- filename: lamini-fine-tuning-api-openapi.yml
  format: yaml
  label: Lamini Fine-Tuning API
  slug: lamini-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-fine-tuning-api-openapi.yml
- filename: lamini-inference-api-openapi.yml
  format: yaml
  label: Lamini Inference API
  slug: lamini-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-inference-api-openapi.yml
- filename: lamini-platform-api-openapi.yml
  format: yaml
  label: Lamini Platform API
  slug: lamini-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lamini.ai
  spf: true
hosts:
- host: www.lamini.ai
  https: false
- cert_expires: Sep 19 03:26:50 2026 GMT
  host: docs.lamini.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 03:26:50 2026 GMT
  host: api.lamini.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lamini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lamini, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lamini
provider_slug: lamini
slug: lamini-domain-security
source_filename: lamini-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lamini.ai\n  https: false\n- host: docs.lamini.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:26:50 2026 GMT\n  hsts: false\n- host: api.lamini.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:26:50 2026 GMT\n  hsts: null\ndomains:\n- domain: lamini.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/security/lamini-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- LLM
- Fine-Tuning
- Memory Tuning
- Inference
---
