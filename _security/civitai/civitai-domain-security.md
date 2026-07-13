---
api_specs:
- filename: civitai-site-api-openapi.yml
  format: yaml
  label: Civitai Site API
  slug: civitai-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-site-api-openapi.yml
- filename: civitai-orchestration-api-openapi.yml
  format: yaml
  label: Civitai Orchestration API
  slug: civitai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-orchestration-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: civitai.com
  spf: true
hosts:
- cert_expires: Oct  4 12:15:38 2026 GMT
  host: civitai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:35:56 2026 GMT
  host: developer.civitai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:36:04 2026 GMT
  host: orchestration.civitai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Civitai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civitai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Civitai
provider_slug: civitai
slug: civitai-domain-security
source_filename: civitai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: civitai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:15:38 2026 GMT\n  hsts: false\n- host: developer.civitai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:35:56 2026 GMT\n  hsts: false\n- host: orchestration.civitai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:36:04 2026 GMT\n  hsts: null\ndomains:\n- domain: civitai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/security/civitai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Artificial Intelligence
- Image Generation
- Video Generation
- Stable Diffusion
- SDXL
- Flux
- LoRA
- Model Hosting
- Community
- Generative AI
---
