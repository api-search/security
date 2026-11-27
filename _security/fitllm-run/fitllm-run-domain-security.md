---
api_specs:
- filename: fitllm-run-api-openapi.json
  format: json
  label: FitLLM Agent API API
  slug: fitllm-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fitllm-run/openapi/_original/fitllm-run-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fitllm.run
  spf: false
hosts:
- cert_expires: Dec 25 19:38:03 2026 GMT
  host: fitllm.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FitLLM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FitLLM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FitLLM
provider_slug: fitllm-run
slug: fitllm-run-domain-security
source_filename: fitllm-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fitllm.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 19:38:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fitllm.run\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fitllm-run/security/fitllm-run-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- LLM
- Calculator
- GPU
- Memory
---
