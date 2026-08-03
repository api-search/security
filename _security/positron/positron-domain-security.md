---
api_specs:
- filename: positron-inference-openapi.yml
  format: yaml
  label: Positron Olivaw OpenAI-Compatible Inference API
  slug: positron-olivaw-openai-compatible-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/openapi/positron-inference-openapi.yml
- filename: positron-admin-openapi.yml
  format: yaml
  label: Positron Olivaw Admin API
  slug: positron-olivaw-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/openapi/positron-admin-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: positron.ai
  spf: true
hosts:
- cert_expires: Sep 23 19:39:59 2026 GMT
  host: www.positron.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 12:06:21 2026 GMT
  host: support.positron.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 06:54:39 2026 GMT
  host: api.positron.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Positron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Positron, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Positron
provider_slug: positron
slug: positron-domain-security
source_filename: positron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.positron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:39:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.positron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:06:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.positron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 06:54:39 2026 GMT\n  hsts: null\ndomains:\n- domain: positron.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/security/positron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- artificial-intelligence
- ai-inference
- inference-hardware
- ai-accelerators
- large-language-models
- transformers
- openai-compatible
- machine-learning
- semiconductors
- data-center
- llm-serving
- model-hosting
---
