---
api_specs:
- filename: siliconflow-openapi.yml
  format: yaml
  label: SiliconFlow Cloud Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: siliconflow.com
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: siliconflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:44:10 2026 GMT
  host: docs.siliconflow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 10:12:23 2026 GMT
  host: api.siliconflow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siliconflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SiliconFlow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SiliconFlow
provider_slug: siliconflow
slug: siliconflow-domain-security
source_filename: siliconflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siliconflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.siliconflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:44:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.siliconflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:12:23 2026 GMT\n  hsts: null\ndomains:\n- domain: siliconflow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/security/siliconflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- LLM
- Inference
- Open Source
- OpenAI Compatible
- Anthropic Compatible
- Image Generation
- Audio
- Video
---
