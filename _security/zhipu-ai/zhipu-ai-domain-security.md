---
api_specs:
- filename: zhipu-ai-openapi.json
  format: json
  label: Z.ai Open Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zhipu-ai/refs/heads/main/openapi/zhipu-ai-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zhipuai.cn
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: z.ai
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.zhipuai.cn
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 07:04:32 2026 GMT
  host: docs.z.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.z.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zhipu Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zhipu AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zhipu AI
provider_slug: zhipu-ai
slug: zhipu-ai-domain-security
source_filename: zhipu-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zhipuai.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: docs.z.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:04:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.z.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zhipuai.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: z.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zhipu-ai/refs/heads/main/security/zhipu-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- GLM
- ChatGLM
- Multimodal
---
