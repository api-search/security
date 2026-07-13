---
api_specs:
- filename: vllm-openapi.yml
  format: yaml
  label: vLLM OpenAI-Compatible Server
  slug: openai-compatible
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vllm/refs/heads/main/openapi/vllm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vllm.ai
  spf: false
hosts:
- cert_expires: Sep 20 20:10:06 2026 GMT
  host: docs.vllm.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vllm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vLLM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: vLLM
provider_slug: vllm
slug: vllm-domain-security
source_filename: vllm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.vllm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:10:06 2026 GMT\n  hsts: false\ndomains:\n- domain: vllm.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vllm/refs/heads/main/security/vllm-domain-security.yml
summary_line: TLSv1.3
tags:
- LLM
- Inference
- Open Source
- GPU
- OpenAI Compatible
- Self-Hosted
---
