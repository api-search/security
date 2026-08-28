---
api_specs:
- filename: localai-api-openapi.yml
  format: yaml
  label: LocalAI API
  slug: localai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localai/refs/heads/main/openapi/localai-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: localai.io
  spf: true
hosts:
- cert_expires: Oct 24 01:25:20 2026 GMT
  host: localai.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Localai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocalAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LocalAI
provider_slug: localai
slug: localai-domain-security
source_filename: localai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 01:25:20 2026 GMT\n  hsts: false\ndomains:\n- domain: localai.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localai/refs/heads/main/security/localai-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Inference
- Self-Hosted
- Open Source
- Agents
- Model Context Protocol
- Speech
- Computer Vision
- Embeddings
- Edge Computing
---
