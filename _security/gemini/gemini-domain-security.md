---
api_specs:
- filename: rest
  format: yaml
  label: Gemini REST API
  slug: gemini-rest-api
  spec_type: OpenAPI
  url: https://generativelanguage.googleapis.com/$discovery/rest?version=v1beta&key=YOUR_API_KEY
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: google.dev
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: ai.google.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: generativelanguage.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gemini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gemini, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gemini
provider_slug: gemini
slug: gemini-domain-security
source_filename: gemini-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai.google.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: generativelanguage.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: google.dev\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemini/refs/heads/main/security/gemini-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Artificial Intelligence
- Audio Understanding
- Batch Processing
- Deep Research
- Document Understanding
- Embeddings
- Function Calling
- Generative Ai
- Image Generation
- Large Language Models
- Machine Learning
- Multimodal
- Structured Output
- Text-To-Speech
- Video Generation
- Video Understanding
---
