---
api_specs:
- filename: hyperbolic-ai-audio-generation-api-openapi.yml
  format: yaml
  label: Hyperbolic Audio Generation API
  slug: hyperbolic-ai-audio-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-ai-audio-generation-api-openapi.yml
- filename: hyperbolic-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Hyperbolic Chat Completions API
  slug: hyperbolic-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-ai-chat-completions-api-openapi.yml
- filename: hyperbolic-ai-completions-api-openapi.yml
  format: yaml
  label: Hyperbolic Completions API
  slug: hyperbolic-ai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-ai-completions-api-openapi.yml
- filename: hyperbolic-ai-image-generation-api-openapi.yml
  format: yaml
  label: Hyperbolic Image Generation API
  slug: hyperbolic-ai-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-ai-image-generation-api-openapi.yml
- filename: hyperbolic-ai-models-api-openapi.yml
  format: yaml
  label: Hyperbolic Models API
  slug: hyperbolic-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-ai-models-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyperbolic.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyperbolic.xyz
  spf: true
hosts:
- cert_expires: Sep 26 05:42:00 2026 GMT
  host: www.hyperbolic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:50:22 2026 GMT
  host: docs.hyperbolic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 13:04:04 2026 GMT
  host: api.hyperbolic.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperbolic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperbolic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hyperbolic
provider_slug: hyperbolic-ai
slug: hyperbolic-ai-domain-security
source_filename: hyperbolic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperbolic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:42:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hyperbolic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:50:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hyperbolic.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:04:04 2026 GMT\n  hsts: null\ndomains:\n- domain: hyperbolic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hyperbolic.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/security/hyperbolic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Compute
- Decentralized
- DePIN
- GPU
- Image-Generation
- Inference
- LLM
- Marketplace
- Open-Source
---
