---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: octo.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: octoai.run
  spf: false
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: octo.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: text.octoai.run
  https: false
- host: image.octoai.run
  https: false
kind: domain-security
layout: security
method: probed
name: Octoai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OctoAI, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OctoAI
provider_slug: octoai
slug: octoai-domain-security
source_filename: octoai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octo.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\n- host: text.octoai.run\n  https: false\n- host: image.octoai.run\n  https: false\ndomains:\n- domain: octo.ai\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: octoai.run\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octoai/refs/heads/main/security/octoai-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Acquired
- Defunct
- AI Inference
- Generative AI
- LLM
- Foundation Models
- Model Optimization
- Apache TVM
- GPU
- Private AI
- NVIDIA
---
